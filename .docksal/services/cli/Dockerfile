FROM docksal/cli:edge-php7.1
RUN \
    apt-get update; \
    apt-get install -y --force-yes --no-install-recommends \
    build-essential chrpath libssl-dev libxft-dev \
    libfreetype6 libfreetype6-dev \
    libfontconfig1 libfontconfig1-dev
ENV PHANTOM_JS="phantomjs-2.1.1-linux-x86_64"
RUN \
    cd /tmp; \
    wget -q https://github.com/Medium/phantomjs/releases/download/v2.1.1/$PHANTOM_JS.tar.bz2 -O $PHANTOM_JS.tar.bz2; \
    tar xvjf $PHANTOM_JS.tar.bz2; \
    mv $PHANTOM_JS /usr/local/share/; \
    ln -sf /usr/local/share/$PHANTOM_JS/bin/phantomjs /usr/local/share/phantomjs; \
    ln -sf /usr/local/share/$PHANTOM_JS/bin/phantomjs /usr/local/bin/phantomjs; \
    ln -sf /usr/local/share/$PHANTOM_JS/bin/phantomjs /usr/bin/phantomjs; \

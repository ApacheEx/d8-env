# d8-env
This is a pure Drupal 8 installation pre-configured for use with Docksal on Drupal Code Sprint.

Features:

- Drupal 8.6.x
- Install Drupal via `fin init`
- Run PHPUnit tests via `fin test`
- Apache 2.4 + MySQL 5.5 + PHP 7.1 + PhantomJs 2.1 + adminer
- PHP and MySQL settings overrides [examples](.docksal/etc)

## Setup instructions

### Step #1: Docksal environment setup

**This is a one time setup - skip this if you already have a working Docksal environment.**  

Follow [Docksal environment setup instructions](https://docs.docksal.io/en/master/getting-started/env-setup)

### Step #2: Project setup

1. The simplest way of configuring env is to execute the following command in your `Projects` directory

   ```
   fin exec-url https://raw.githubusercontent.com/ApacheEx/d8-env/master/.docksal/commands/web-init
   ```
   
   When the automated install is complete the command line output will display the admin username and password.

2. Point your browser to

   ```
   http://d8.docksal
   ```
   
3. Check the [wiki-page](https://github.com/ApacheEx/d8-env/wiki) for more info.


## Note

This repo is intended for quick start on Drupal Code Sprint.

## License

MIT © [Oleg Kuzava](https://github.com/ApacheEx)

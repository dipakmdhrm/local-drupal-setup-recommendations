# Apps
## Must haves:
### Xcode:
  - IDE (Integrated development environment) and CLT(Command line tools) for MacOS.
  - Installing this will install tools like git, compilers for languages etc.
  - Installation:
    - Open terminal and run the following command:
      - `xcode-select --install`
### Homebrew (`brew`)
  - Package installer for MacOS.
  - Installing this will allow you to install system apps an programs. Eg. PHP, composer, Mysql, etc.
  - Installation:
    - Open terminal and run the following command:
      - `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`
    - Or find the latest installation instructions at: `https://brew.sh/`
### IDE/Code editor:
  - PHPStorm:
    - Better than every other PHP IDE.
    - Go for it only if you have the license.
  - VS Code:
    - Installation:
      - Download and install from:
        - https://code.visualstudio.com/
      - Or via Homebrew in terminal:
        - `brew update`
        - `brew tab caskroom/cask`
        - `brew cask install visual-studio-code`
### SequelPro:
  - DBMS (DataBase Management System)
  - Installation:
    - Download & install from:
      - https://sequelpro.com/
### Composer:
  - PHP Package manager:
  - Installation:
    - Follow instructions at https://getcomposer.org/download/
    - Or via Homebrew in terminal:
      - `brew install composer`
  - Usage:
    - Run the following commands in terminal:
      - `composer global require {xxxx}/{yyyy}` for globally installing a package named yyyy from xxxx vendor.
      - `composer require {xxxx}/{yyyy}` for installing a package named yyyy from xxxx vendor in the current directory only.
### Composer global packages:
  - **Drush:**
    - Drupal CLI
    - Installation:
      - Via composer in terminal:
        - `composer global require drush/drush`
  - **Drupal Coder:**
    - PHPCS coding standards for Drupal
    - PHPCS: PHP Code Sniffer. Parses PHP files to check code standard violations. Example standards:
      1. PSR-1
      2. PSR-2
      3. PSR-12
      4. PEAR
      5. Zend
      6. Drupal
      7. DrupalPractice
    - Installation:
      - Via composer in terminal:
        - `composer global require drupal/coder`
    - Usage:
      - Run the following command in terminal for a file to show violations:
        - `phpcs --standard=Drupal file.php` for coding standard violations
        - `phpcs --standard=DrupalPractice file.php` for bad practices
        - `phpcs --standard=Drupal,DrupalPractice file.php` for both

## Recommended:
### Mysql:
   1. Most widely used DataBase & query language. There are 90% changes you're using this in your project.
   2. Installation:
      1. Via Homebrew in terminal:
         1. `brew install mysql` (or `brew install mysql@5.7` for specific version. Replace 5.7 with version you want)
### VirtualBox:
  - PC virtualization software.
  - A lot of project use drupal-vm based local setup. DrupalVM relies on VirtualBox for the 'VM' part which makes this a necessity:
  - Installation:
    - Download and install from:
      - https://www.virtualbox.org/wiki/Downloads
    - Or via Homebrew in terminal:
      - `brew update`
      - `brew tab caskroom/cask`
      - `brew cask install virtualbox`
### Password Manager:
  - Lastpass
### GIMP:
  - Photoshop alternative
### Postman:
  - API Client
  - Supports REST, GraphQL, SOAP etc
### Nodejs:
   - nvm is recommended managing different versions of nodes

## Optional:
### VPN:
  - ProtonVPN
### Multiple Web browsers:
  - Note: You can install multiple versions of browsers:
    - Google chrome:
      - Stable: https://www.google.com/chrome/
      - Beta: https://www.google.com/chrome/beta/
      - Canary: https://www.google.com/chrome/canary/
      - Chromium: https://chromium.woolyss.com/download/#mac
    - Firefox:
      - Stable: https://www.mozilla.org/en-GB/firefox/download/thanks/
      - Beta: https://www.mozilla.org/en-US/firefox/channel/desktop/
      - Developer edition: https://www.mozilla.org/en-US/firefox/channel/desktop/
      - Nightly: https://www.mozilla.org/en-US/firefox/channel/desktop/

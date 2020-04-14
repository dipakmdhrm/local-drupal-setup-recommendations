# IDE / Text editor configurations

## Choosing a code editor for Drupal/PHP development.
- PHPSTORM is the best tool for any kind of PHP development. Go for it if you can **legally** obtain a license.
- VSCODE is next best alternative and the one I would personally recommend.
- Honorable mention: Sublime text.

## VSCODE configuration recommendations:

### Must haves:
1. Install code in commandline:
   1. CMD + Shift + P:
      1. Choose "install 'code' command in path"
2. Get familiar with VSCode settings:
   1. UI: Code > Preferences > Settings
   2. File: `settings.json`
3. Optimize you IDE for Drupal Coding standards:
   1.  https://www.drupal.org/docs/develop/development-tools/configuring-visual-studio-code
4. Recommended Plugins (VS Code):
   1. **PHP Extenstion Pack:**
      1. Basic PHP support. Needed for other plugins.
   2. **PHP IntelliSense:**
      1. Autocompletion
      2. Signature Help
      3. Goto Definition etc.
   1. **Drupal Syntax Highliting:**
      1. Adds syntax highliting for Drupal specific file extenstions:
         1. `.install`
         2. `.module`
         3. `.theme` etc
   2. **Drupal 8 Snippets/Drupal 8 Snippets (Advanced):**
      1. Add snippents for hooks
   3. **Twig:**
      1. For twig syntax highliting
   4. **PHPCS:**
      1. Code Linting: Showing errors in code in real-time.
      2. Configure in `settings.json` to use `Drupal` & `DrupalPractice` Standard.
      3. PHPCS should be installed on your system for this to work.
   5. **PHPDocBlocker:**
      1. Adds docblock snippets based on context if you type `/**` and press enter above a class, function, class property etc.
   6. **PHP Debug:**
      1. Xdebug Client/Adapter for VSCode
      2. Allows users to step-debug PHP code.
      3. Prerequisites:
         1. Xdebug should be installed on system
         2. Following xdebug config should be enabled in `php.ini`:
            1. `xdebug.remote_enable = 1`
            2. `xdebug.remote_autostart = 1`
      4. Configuration:
         1. Create `launch.json` with default configuration for xdebug installed on local system.
         2. Create `launch.json` with default configuration + extra `pathMapping` configuration for xdebug installed in VM or container.

### Recommended:

### Optional:

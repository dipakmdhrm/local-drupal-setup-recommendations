# Drupal configuration for local setup

## Development settings.php & services.yml
1. It is recommended to keep different sets of `settings.php` & `services.yml` for local and other environments.
   1. Local `settings.php` should be a copy of `example.settings.local.php`
   2. Local `services.yml` should be a combination of `default.services.yml` & `development.services.yml`
2. It is recommended not commit `settings.php` to codebase.
   1. This allows develeoper to include `local.settings.php` in their `settings.php`
   2. This also allows TL/TA to include respective settings & services on TEST/PROD environments.
3. In local `settings.php`:
   1. It is recommended to keep the following caches pointed to null during development.
      1. `$settings['cache']['bins']['render']`
      2. `$settings['cache']['bins']['page']`
      3. `$settings['cache']['bins']['dynamic_page_cache']`
   2. It is recommended to keep the css/js aggregation turned off for local:
      1. `$config['system.performance']['css']['preprocess'] = FALSE;`
      2. `$config['system.performance']['js']['preprocess'] = FALSE;`
4. In local `services.yml` :
   1. It is recommended to keep:
      1. Twig debugging as `true`
      2. Twig caching as `false`

## Recommended devlopment modules:
### Core modules:
1. **Database logging:**
   1. For error logging
2. **Syslog:**
   1. For error logging:
      1. Usually catches logs missed by Database logs
### Contrib modules:
1. Devel suite:
   1. **Devel Generate:**
      1. Generates dummy content for testing
   2. **Kint:**
      1. Debugging code
   3. **WebProfiler:**
      1. Page performance
2. **XHProf:**
   1. PHP performance
   2. XHProf PHP extenstion needs to installed
   3. Having an XHProf UI is recommended
3. **Stage File Proxy:**
   1. Servers Production files (Images, videos) on local
4. **Admin Toolbar & Admin Toolbar extras:**

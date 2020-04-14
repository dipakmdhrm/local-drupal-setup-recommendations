# Drupal Installation:

3 options:
### AMP stack installed on your system directly:
1. **Examples:**
    1. Bare bones MacOS (Recommened for learning purposes):
      1. Apache & PHP come pre-installed
      2. Just Mysql needs to installed. Use brew.
    2. XAMPP:
      3. Installs Apache, PHP & Mysql
    3. MAMP/MAMP PRO (Recommended if you can obtaina a license **legally**):
      4. Installs Apache, PHP & Mysql
    4. Acquia Dev Desktop:
      5. Installs Apache, PHP & Mysql
2. **Pros:**
    1. Superfast websites.
3. **Cons:**
    1. A lot of manual configuration:
          1. Creating vhosts in apache config (Not in MAMP PRO)
          2. Installation of packages like:
            1. Xdebug
            2. Xhprof
            3. Solr
            4. Memcache etc.
          3. Integration with build tools (BLT)
4. **Recommended for:**
   1. Small sites
   2. Personal projects
   3. Contrib work
### Container (Usually Docker) based options:
1. **Examples:**
   1. Docksal
   2. DDev
   3. Lando
2. **Pros:**
   1. Easy configuration for automating many things:
      1. Creating vhosts
      2. Installation of packages
   2. Fast (still slower than AMP stack installed directly on system)
   3. Good support for build tools (BLT)
3. **Cons:**
   1. Learning curve
4. **Recommended for:**
   1. Medium to Large sites
   2. Sites with lots of integrations (Solr, Memcache etc.)
### Virtual Machine based options:
1. **Examples:**
   1. Drupal VM (Most popular option)
2. **Pros:**
   1. YML based configuration for automating many things:
      1. Creating vhosts
      2. Installation of packages
   2. Good support for build tools (BLT)
   3. Very good community support (Best in business)
3. **Cons:**
   1. Learning curve
   2. Slowest in bunch.
4. **Recommended for:**
   1. Medium to Large sites
   2. Sites with lots of integrations (Solr, Memcache etc.)

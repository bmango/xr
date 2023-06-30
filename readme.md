1. $ git clone xxx .
2. $ cd dir
3. $ composer update
4. $ echo '$settings["config_sync_directory"] = "../config/sync";' >> web/sites/default/default.settings.php
5. cd web
6. $ drush si -vv --site-name[=SITE-NAME] --site-pass=[PASSWORD] --db-url=mysql://db_name:password@localhost:3306/db_name
7. $ drush si --existing-config


Note - 
Before starting need to be using at least php 8.0, recent version of composer and drush - drush will come after step 3, when you run 'composer update' and is located at '/vendor/drush/drush/drush', so a sample drush command might be:

'/usr/local/bin/ea-php81 -d memory_limit=2048M ~/public_html/dir/vendor/drush/drush/drush si -vv --existing-config'

a sample composer command might be:

'/usr/local/bin/ea-php81 -d memory_limit=2048M ~/bin/composer update'

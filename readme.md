1. $ git clone xxx .
2. $ cd dir
3. $ composer update
4. $ echo '$settings["config_sync_directory"] = "../config/sync";' >> web/sites/default/default.settings.php
5. cd web
6. $ drush si -vv --site-name[=SITE-NAME] --site-pass=[PASSWORD] --db-url=mysql://db_name:password@localhost:3306/db_name
7. $ drush si --existing-config

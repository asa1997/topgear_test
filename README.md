
|# |Input parameter name / output field |Description |Host env var |Ansible var name  |BeSman script vars |Type |Default | |
|:----|:----|:----|:----|:----|:----|:----|:----|:----|
| | | | | | |(Mandatory/optional) | | |
|1 |User name |User with permission to launch oah environments |OAH_USER |oah_user |BES_USER |M |Picks up current user or sets to vagrant | |
|2 |Vagrant box name |Specifies OS type for the VM |vagrant_box |vagrant_box |NA |M |hashicorp/bionic64| |
|3 |Vagrant root user |The root user of the VM |vagrant_user |vagrant_user |NA |M |vagrant | |
|4 |Host name |The name of the host vm |vagrant_hostname |vagrant_hostname |NA |M |oah-bes-vm| |
|5 |Webserver |The web server software to use. |drupalvm_webserver |oah_env_webserver |BESMAN_ENV_WEBSERVER |O |Apache| |
|6 |database |The database system to use. |drupal_db_backend |oah_env_db_backend |BESMAN_ENV_DB_BACKENED |O |mysql| |
|7 |Build composer flag |Setting this flag to true allows the user to install drupal using composer |drupal_build_composer |oah_build_composer |BESMAN_ENV_BUILD_COMPOSER |O |false | |
|8 |composer. json path |Path under which composer.json fie resides |drupal_composer_path |oah_composer_path |BESMAN_ENV_COMPOSER_PATH |O |Inside the provisioned Drupal environment | |
|9| drupal composer package|Version of drupal code base that composer downed.  | drupal_composer_project_package|oah_composer_project_package| BESMAN_ENV_COMPOSER_PROJECT_PACKAGE|o| drupal/recommended-project:^9@dev| |
|10|drupal install directory  path|Setting path under which drupal get installed. |drupal_composer_install_dir|oah_composer_install_dir| BESMAN_ENV_COMPOSER_INSTALL_DIR|O |/var/www/html/drupal| |
|11|Drupal project relase options|select the type of relase package(stable, dev etc. )|drupal_composer_project_options|oah_composer_project_options|BESMAN_ENV_COMPOSER_PROJECT_OPTIONS|O|-prefer-dist --stability dev --no-interaction'| |
|12|Druapal install site|Set this to 'false' if you don't need to install drupal (using the drupal_*settings below), but instead copy down a database (e.g. using drush sql-sync).|drupal_install_site|oah_install_site|BESMAN_ENV_INSTALL_SITE|O| true| |
|13|Druapl app data path|Main Drupal data path|drupal_core_path|oah_core_path|BESMAN_ENV_CORE_PATH|M |/var/www/drupal/web| |
|14|Drupal user|Drupal user with admin privilage |drupal_core_owner|oah_core_owner|BESMAN_ENV_CORE_OWNER|M |vagrant | |
|15|Druapal data base user name|data base username|drupal_db_user|oah_db_user|BESMAN_ENV_DB_USER|M |drupal| |
|16|Druapal data base password|data base password|drupal_db_password|oah_db_password|BESMAN_ENV_DB_PASSWORD|M |drupal| |
|17|Drupal DB name|data base name of drupal app|drupal_db_name|oah_db_name|BESMAN_ENV_DB_NAME|M |drupal| |
|18|Drupal hostname|host/hostname for drupal|drupal_db_host|oah_db_host|BESMAN_ENV_DB_HOST|M |localhost| |
|19|Latest stable version details|Latest major version of Drupal application|drupal_major_version|oah_major_version|BESMAN_ENV_MAJOR_VERSION|O|latest version (Currnet 9)| |
|20|Domain for Drupal|Domain name Drupal |drupal_domain|oah_domain|BESMAN_ENV_DOMAIN|O|oah-bes-vm| |
|21|Site name|Drupal site name|drupal_site_name|oah_site_name|BESMAN_ENV_SITE_NAME|O|Drupal| |
|22|Profile set up|Provision for setting drupal profile while install |drupal_install_profile|oah_install_profile|BESMAN_ENV_INSTALL_PROFILE|O|standard| |
|23|Drupal module list|List of module names to be work with drupal |drupal_enable_modules|oah_enable_modules|BESMAN_ENV_ENABLE_MODULES|O|devel| |
|24|Drupal account username|Drupal app account user name|drupal_account_name|oah_account_name|BESMAN_ENV_ACCOUNT_NAME|O|admin| |
|25|Drupal account password|Drupal app account user password|drupal_account_pass|oah_account_pass|BESMAN_ENV_ACCOUNT_PASS|O|admin| |
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

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
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

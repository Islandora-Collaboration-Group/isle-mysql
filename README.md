# ISLE MySQL

## Part of the ISLE Islandora 7.x Docker Images

* Designed as the MySQL database search server for ISLE. It hosts the Drupal and Fedora databases.

Based on:

* [MySQL 5.7](https://hub.docker.com/_/mysql)

Contains and Includes:
* [MySQL 5.7](https://hub.docker.com/_/mysql)
* ISLE.cnf (_found at /etc/mysql/mysql.conf.d/ISLE.cnf_)
  - Default ISLE MySQL configuration file for MySQL server usage with additional parameters
  - builds on the default MySQL configuration file (_found at /etc/mysql/mysql.conf.d/mysqld.cnf_)

## Environmental Variables Available:

At the top of each [ISLE](https://github.com/Islandora-Collaboration-Group/ISLE) `.env` file (_e.g. local.env, staging.env etc_), there is the `## Database (SQL)` section which contains multiple environemental variables that impact this image / container / service.

* `MYSQL_ROOT_PASSWORD=`
  * This variable is mandatory and specifies the password that will be set for the MySQL root superuser account.
  * Replace the comment line to the right of the `=` (#...) with a recommended password of 26 alpha-numeric characters

* `FEDORA_DB=fedora3`
  * This variable is mandatory / fixed and specifies the Fedora database name. Please do not change it.

* `FEDORA_DB_USER=fedora_admin`
  * This variable is mandatory / fixed and specifies the Fedora database user. Please do not change it.

* `FEDORA_DB_PASS=`
  * This variable is mandatory and specifies the password that will be set for the Fedora database user account.
  * Replace the comment line to the right of the `=` (#...) with a recommended password of 26 alpha-numeric characters

* `DRUPAL_DB=`
  * This variable is mandatory and specifies the Drupal database name.
  * Replace the comment line to the right of the `=` (#...) with a easy to read but short database name e.g. acmeco_db or institution_db

* `DRUPAL_DB_USER=`
  * This variable is mandatory and specifies the Drupal database user name.
  * Replace the comment line to the right of the `=` (#...) with a easy to read but short database user e.g. acmeco_db_user or institution_db_user

* `DRUPAL_DB_PASS`
  * This variable is mandatory and specifies the Drupal database user password.
  * Replace the comment line to the right of the `=` (#...) with a recommended password of 26 alpha-numeric characters

## License

* For the MySQL portion of this image, refer to https://hub.docker.com/_/mysql: "View [license](https://www.mysql.com/about/legal/) information for the software contained in this image."

* For all other configuration or changes to this image are subject to the [LICENSE](LICENSE) file

## Usage

* For general usage of this image and [ISLE](https://github.com/Islandora-Collaboration-Group/ISLE), please refer to [ISLE documentation](https://islandora-collaboration-group.github.io/ISLE/)
# ISLE MySQL

## Part of the ISLE Islandora 7.x Docker Images

* Designed as the MySQL database search server for ISLE. It hosts the Drupal and Fedora databases.

Based on:
  - [MySQL 5.7](https://hub.docker.com/_/mysql)

Contains and Includes:
  - [MySQL 5.7](https://hub.docker.com/_/mysql)
  - ISLE.cnf (_found at /etc/mysql/mysql.conf.d/ISLE.cnf_)
    - Default ISLE MySQL configuration file for MySQL server usage with additional parameters
    - builds on the default MySQL configuration file (_found at /etc/mysql/mysql.conf.d/mysqld.cnf_)
  
## Usage

* For general usage of this image and [ISLE](https://github.com/Islandora-Collaboration-Group/ISLE), please refer to [ISLE documentation](https://islandora-collaboration-group.github.io/ISLE/)
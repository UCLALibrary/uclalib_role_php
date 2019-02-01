uclalib_role_php
=========

Dependencies
------------

None.

Example Playbook
----------------

A sample is provided below including variables with a list of PHP packages within the playbook file:

    - hosts: all
      vars:
        php_pkgs:
          - php
          - php-ldap
          - php-cli
          - php-xml
          - php-mysql
          - php-pecl-memcache
          - php-pecl-apc
          - php-gd
          - php-mcrypt
          - php-pear
          - php-pdo
          - php-mbstring
          - php-common
          - php-phpseclib-crypt-hash
      roles:
          - { role: uclalib_role_php }
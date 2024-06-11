uclalib_role_php
=========

Ansible role to install PHP on a RHEL8 system.

Requirements
------------

None.

Role Variables
--------------

* `php_version` - defines the version of PHP to install; must be a version available as a RHEL8 module (e.g. `7.2`, `7.3`, `7.4`, `8.0`, `8.2`)
* `php_pkgs` - defines a list of PHP packages to install; unless you are using the default PHP module, the first list item must define the module version (e.g. `@php:7.3`)

Example Playbook
----------------

Define `php_version` and `php_pkgs` in host_vars or group_vars. 

    - hosts: all
      roles:
          - { role: uclalib_role_php }
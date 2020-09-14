ansible-role-mysql
=============

Use this role to install mysql/mariadb on your debian or ubuntu server.

Requirements
------------

This role requires debian or ubuntu.

Role Variables
--------------

The default set of variables defines the percona installation and needs at best to be overwritten in group_vars/host_vars

    mysql_version: 'mariadb' # 'mysql'

The following mandatory variables need to be set in group_vars/host_vars

    mysql_root_password: SOMELONGPASSWORD



Example Playbook
----------------

    - hosts: mysql-server
      roles:
         - ansible-role-mysql

License
-------

MIT

Author Information
------------------
https://github.com/pasernik

Based on https://github.com/andrelohmann/ansible-role-percona_mysql

Mongodb
=========

Ansible role for installing mongodb. Tested platforms are:
* Debian 8
* Debian 9
* Ubuntu 16

Requirements
------------

Debian 8 (jessie)
Debian 9 (stretch)
Ubuntu 16 (xenial)

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

| Parameter | Required | Default | Choices | Comments |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| default_mongodb_admin_db | yes | admin | | Create MongoDB administrator db |
| default_mongodb_root_login | yes | root | | Sets MongoDB user root login |
| default_mongodb_root_password | yes | access | | Sets MongoDB user root password |
| default_mongodb_user_login | yes | user | | Sets default MongoDB user name |
| default_mongodb_user_password | yes | access | | Sets default MongoDB user password |
| default_mongodb_port | yes | 27017 | | Sets MongoDB server port |


Dependencies
------------

None

Example 
----------------
    ---
    - hosts: all
      roles:
         - { role: antonchernik.mongodb }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2017 by [Anton Chernik](https://github.com/antonchernik).

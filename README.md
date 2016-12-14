Ansible Role: PHP Composer
===

[![Build Status](https://travis-ci.org/mm0/ansible-role-php-composer.svg?branch=master)](https://travis-ci.org/mm0/ansible-role-php-composer)

An Ansible role that installs and configures PHP Composer


Requirements
--

PHP

Role Variables
---

Available variables are listed below, there are no defaults:

```yml
configure_composer_key: false # whether to setup a github oauth token

github_oauth_key: 123 # oauth token to use 
```

Dependencies
---

None 

Example Playbook
---

```yml
- hosts: webservers
  vars:
  - { role: ansible-role-php-composer,
      configure_composer_key: true,
      github_oauth_key: 123
    }
```

License
---------------

BSD-2

Author Information
------------------

[Matt Margolin](mailto:matt.margolin@gmail.com)

[mm0](https://github.com/mm0) on github

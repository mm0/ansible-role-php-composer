# README.md

# Ansible Role: PHP Composer

An Ansible role that installs and configures PHP Composer


![travis-ci](https://travis-ci.org/mm0/ansible-role-php-composer.svg?branch=master)

## Requirements

PHP

## Role Variables

Available variables are listed below, there are no defaults:

    configure_composer_key: false # whether to setup a github oauth token

    github_oauth_key: 123 # oauth token to use 


## Dependencies

None 

## Example Playbook

    - hosts: webservers
      vars:
      - { role: ansible-role-php-composer,
          configure_composer_key: true,
          github_oauth_key: 123
        }

## License

MIT

Author Information
------------------

[Matt Margolin](mailto:matt.margolin@gmail.com)

mm0 on github

# Ansible Role: mariadb

[![Build Status](https://travis-ci.org/arillso/ansible.mariadb.svg?branch=master)](https://travis-ci.org/arillso/ansible.mariadb) [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://sbaerlo.ch/licence) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-mariadb-blue.svg)](https://galaxy.ansible.com/arillso/mariadb)

## Description

installs and configures MariaDB.

## Installation

```bash
ansible-galaxy install arillso.mariadb
```

## Requirements

## Role Variables

| Variable             | Default     | Comments (type)                                   |
| :---                 | :---        | :---                                              |
| mariadb_version | 10.2 | mariadb version |
| mariadb_datadir | /var/lib/mysql | mariadb data location |
| mariadb_bind_address | 127.0.0.1 | mariadb bind address |
| mariadb_bind_port | 3306 | mariadb bind port |

## Dependencies

None

## Example Playbook

```yml
- hosts: all
  roles:
     - arillso.mariadb
```

## Changelog

### 1.2.1

* add support for Ubuntu 18.04

### 1.2

* add plugin-load-add
* change flush handlers

### 1.1

* fix errors
* add official MariaDB Repository

### 1.0

* inital role

## Author

* [Simon Bärlocher](https://sbaerlocher.ch)

## License

This project is under the MIT License. See the [LICENSE](https://sbaerlo.ch/licence) file for the full license text.

## Copyright

(c) 2017, Simon Bärlocher
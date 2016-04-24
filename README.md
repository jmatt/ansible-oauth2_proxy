ansible-oauth2_proxy
====================

[![Build Status](https://travis-ci.org/jmatt/ansible-oauth2_proxy.svg?branch=master)](https://travis-ci.org/jmatt/ansible-oauth2_proxy)

Install and configure oauth2_proxy for LSST SQuaRE infrastructure.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: jmatt.oauth2_proxy }


Variables
---------

Variables can be found in [vars/main.yml](https://github.com/jmatt/ansible-oauth2_proxy/blob/master/vars/main.yml) and [defaults/main.yml](https://github.com/jmatt/ansible-oauth2_proxy/blob/master/defaults/main.yml).

License
-------

The MIT License. See the [LICENSE file](https://github.com/lsst-sqre/ansible-oauth2_proxy/blob/master/LICENSE).

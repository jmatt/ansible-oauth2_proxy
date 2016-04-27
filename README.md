ansible-oauth2_proxy
====================

[![Build Status](https://travis-ci.org/lsst-sqre/ansible-oauth2_proxy.svg?branch=master)](https://travis-ci.org/lsst-sqre/ansible-oauth2_proxy)

Install and configure [oauth2_proxy](https://github.com/bitly/oauth2_proxy) for LSST SQuaRE infrastructure.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: lsst-sqre.oauth2_proxy }

Variables
---------

For complete documentation on options see the [oauth2_proxy documentation](https://github.com/bitly/oauth2_proxy#command-line-options). This role only implements a subset of options. These options are not passed as command line options but are instead put into a configuration file at `/etc/oauth2_proxy/oauth2_proxy.conf` using a template.

`oauth2_proxy_client_id` *(required)* The oauth2_proxy client-id option.

`oauth2_proxy_client_secret` *(required)* The oauth2_proxy client-secret option.

`oauth2_proxy_cookie_secret` *(required)* The oauth2_proxy client-secret option.

`oauth2_proxy_cookie_domain` *(default "")* The oauth2_proxy cookie-domain option.

`oauth2_proxy_cookie_expire` *(default "730h")* The oauth2_proxy cookie-expire option.

`oauth2_proxy_cookie_name` *(default "_oauth2_proxy")* The oauth2_proxy cookie-name option.

`oauth2_proxy_cookie_secure` *(default true)* The oauth2_proxy cookie-secure option.

`oauth2_proxy_email_domains` *(list, default \["*\**"\])* The oauth2_proxy email-domains option.

`oauth2_proxy_github_org` *(default "")* The oauth2_proxy github-org option.

`oauth2_proxy_pass_access_token` *(default false)* The oauth2_proxy pass-access-token option.

`oauth2_proxy_pass_host_header` *(default true)* The oauth2_proxy pass-host-header option.

`oauth2_proxy_provider` *(default "github")* The oauth2_proxy provider option.

License
-------

The MIT License. See the [LICENSE file](https://github.com/lsst-sqre/ansible-oauth2_proxy/blob/master/LICENSE).

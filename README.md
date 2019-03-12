Ansible Role: Netatalk
=========

[![Build Status](https://travis-ci.org/michalschott/ansible-role-netatalk.svg?branch=master)](https://travis-ci.org/michalschott/ansible-role-netatalk)

Simple ansible role, which can be run on `Ubuntu 14.04/16.04/18.04` to:
- build netatalk (http://netatalk.sourceforge.net) service from source code
- pack it into .deb archive using checkinstall
- install it on the same system
- create directory and expose it for Time Machine Backups

Requirements
------------

None.

Role Variables
--------------

Default variables:
```
netatalk_version: '3.1.11'
netatalk_url: 'http://prdownloads.sourceforge.net/netatalk/netatalk-{{ netatalk_version }}.tar.gz?download'
netatalk_timemachine_path: /mnt/TimeMachine
netatalk_timemachine_vol_size_limit: 512000
netatalk_timemachine_valid_users:

```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: netatalk }

License
-------

MIT

Author Information
------------------

This role was created in 2016 by [Michal Schott](http://github.com/michalschott).

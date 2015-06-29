Role Name
=========

Ansible role to setup SSH Authentication via [hesiod](https://en.wikipedia.org/wiki/Hesiod_(name_service)) DNS lookup.

Requirements
------------

Suggested to be used in conjunction with [hesiod53](https://github.com/fullcontact/hesiod53) to create the DNS records on AWS Route53, but could be used stand alone.

Role Variables
--------------

You can find variable defaults in `defaults/*` however the ones you'll have to edit are `defaults/hesiod_conf.yml`

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: fullcontact.hesiod }

License
-------

MIT

Author Information
------------------

FullContact
https://github.com/fullcontact/
ops+hesiod53@fullcontact.com

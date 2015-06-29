Role Name
=========

Ansible role to setup SSH Authentication via [hesiod](https://en.wikipedia.org/wiki/Hesiod_(name_service)) DNS lookup.

Requirements
------------

Suggested to be used in conjunction with [hesiod53](https://github.com/fullcontact/hesiod53) to create the DNS records on AWS Route53, but could be used stand alone.

Role Variables
--------------

You can find variable defaults in `defaults/main.yml`. Main ones you want to edit are

```
hesiod_conf_lhs: '.hesiod'
hesiod_conf_rhs: '.yourdomain.com'
```


Example Playbook
----------------

```
    - hosts: servers
      roles:
         - role: riltsken.hesiod
           hesiod_conf_lhs: '.hesiod'
           hesiod_conf_rhs: '.yourdomain.com'
```

License
-------

MIT

Author Information
------------------

FullContact

https://github.com/fullcontact/

ops+hesiod53@fullcontact.com

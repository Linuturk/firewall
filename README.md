firewall
========

[![Build Status](https://drone-opsdev.rax.io/github.com/rack-roles/firewall/status.svg?branch=master)](https://drone-opsdev.rax.io/github.com/rack-roles/firewall)

Uses the Ansible ufw module to manage firewall rules.

Requirements
------------

UFW

Role Variables
--------------

* `firewall_allowed_services` Only supported on Ubuntu. List service names (ie, OpenSSH)
* `firewall_allowed_ports` Define a list of hashes that specify port and proto.

```
firewall_allowed_ports:
  - port: 80
    proto: tcp
```

Dependencies
------------

None

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: Rackspace_Automation.firewall, x: 42 }

License
-------

BSD

Author Information
------------------

[Rackspace - the open cloud company](http://rackspace.com)

Ask about our DevOps Automation Service - [www.rackspace.com/devops](http://rackspace.com/devops)

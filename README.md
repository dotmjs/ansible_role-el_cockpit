dotmjs.el_cockpit
=========

A role to install and configure Cockpit (https://cockpit-project.org/) on an EL host, including optional configuration of non-standard port.

Requirements
------------

- libselinux-python: must be installed to support changing selinux context for custom port
- Tested on CentOS8 Stream and Fedora 34

Role Variables
--------------

cockpit_port: If not set set, cockpit will use the default TCP\9090.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: dotmjs.el_cockpit, cockpit_port: 9091 }

License
-------

BSD

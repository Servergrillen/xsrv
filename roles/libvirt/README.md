libvirt
=============

This role will install and configure [libvirt], a collection of software that provides a convenient way to manage virtual machines and other virtualization functionality, such as storage and network interface management.


Requirements
------------

- Ansible 2.10 or higher on ansible controller
- Debian GNU/Linux 10 on host


Configuration variables
-----------------------

See [defaults/main.yml](defaults/main.yml)


Example playbook
-----------------

```yaml
- hosts: my.example.org
  roles:
     - libvirt
  vars:
```


Usage
------------


License
-------

[GNU GPLv3](../../LICENSE)

References
-----------------

- https://stdout.root.sx/links/?searchterm=libvirt
- https://stdout.root.sx/links/?searchtags=virtualization


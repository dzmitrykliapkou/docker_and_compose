Docker and docker-compose
=========

This Ansible role installs docker using apt, yum or amazon-linux-extras depending on OS family and distribution name. Also the role downloads specified or latest docker-compose version.

Requirements
------------

None.

Role Variables
--------------

| Variable                | Description                                | Default value                   |
| :---------------------- | :----------------------------------------- | :------------------------------ |
| docker_compose_path     | Path to place docker-compose binary        | `/usr/local/bin/docker-compose` |
| docker_compose_version  | Specific docker-compose version to install | latest                          |

Dependencies
------------

None.

Example Playbook
----------------

```yaml
    - hosts: localhost
      roles:
         - role: docker_and_compose
```

License
-------

[GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)

Author Information
------------------

[Dzmitry Kliapkou](https://github.com/dzmitrykliapkou)

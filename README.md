Ansible role: PHP RoadRunner
=========

Ansible roles to install rr binary globally. [RoadRunner] is a high-performance PHP application server, load-balancer, and process manager written in Golang. Most of the process using same as a mention in official documentation to install manually using curl.

Requirements
------------

Require to install gnu-tar in macOS, use `brew install gnu-tar` to install.

Role Variables
--------------

List of variables in ansible-role-php-roadrunner:

```sh
rr_repo_base: "https://api.github.com/repos/roadrunner-server/roadrunner"
rr_version: "latest"
rr_token: ""
rr_name: "roadrunner"
rr_arch_type:
  - { key: "aarch64", value: "arm64" }
  - { key: "x86_64", value: "amd64" }
  - { key: "arm64", value: "arm64" }
```


Dependencies
------------

None.

Example Playbook
----------------

```sh
- hosts: servers
  roles:
    - ansible-role-php-roadrunner
```

License
-------

MIT

Author Information
------------------

[Nedya Prakasa]. Role created for [dPanel].

[dPanel]: https://cloud.terpusat.com/
[Nedya Prakasa]: https://github.com/prakasa1904
[mit]: https://opensource.org/licenses/MIT
[RoadRunner]: https://roadrunner.dev/
[devetek]: https://github.com/devetek
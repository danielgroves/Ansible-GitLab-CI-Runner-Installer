# Ansible GitLab CI Runner Installer

Installs the GitLab CI Runner as par the instructions provided.

To use, simply add as a sub-repository or clone into your project and pass in the required variables below.

* `ci_server`: The full URL for the server, including http(s)://
* `ci_token`: The registration token provided by GitLab CI
* `ci_ssh_server`: The SSH address for the server, normally the same as the ci_server address.

The example configuration below shows example values.

```
- hosts: all
  roles:
      - { role: gitlab-ci-runner,
          ci_server: "http://ci.example.com",
          ci_token: "f31abbde917e74d6f517",
          ci_ssh_server: "ci.example.com" }
```

The playbook is MIT licensed. See LICENSE for full details.

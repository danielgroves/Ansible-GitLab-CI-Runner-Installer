# Ansible GitLab CI Runner Installer

Installs the GitLab CI Runner as par the instructions provided.

To use, simply add as a sub-repository or clone into your project and configure with the variable shown below.

```
- hosts: all
  roles:
      - { role: gitlab-ci-runner, ci_server: "WEB ADDRESS FOR YOUR SERVER", ci_token: "THE TOKEN GIVEN BY GITLAB CI", ci_ssh_server: "THE DOMAIN AGAIN, WITHOUT http(s)://" }
```

A decent read me will appear once the ruby problems have been fixed. 

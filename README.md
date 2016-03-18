# Another Docker ansible role

It currently only supports RHEL/CentOS 7.x  
Major difference with other available Docker roles is that this one can configure Docker to listen on TCP...   

## Example Playbook
```
- hosts: servers
  roles:
    - { role: sebbrochet.docker, docker_tcp: true }
```

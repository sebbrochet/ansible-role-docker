# Another Docker ansible role

It currently only supports RHEL/CentOS 7.x  
Major difference with other available Docker roles is that this one can configure Docker to listen on TCP...   

## Installation

* Put these lines in your `requirements.yml` file:   
  ```
  - src: https://github.com/sebbrochet/ansible-role-docker
    version: master
    name: docker
  ```
* Get the code with ansible-galaxy   
  `ansible-galaxy -r requirements.yml`

## Example Playbook
```
- hosts: servers
  roles:
    - { role: docker, docker_tcp: true }
```

## jenkins-swarm

[![Travis CI](http://img.shields.io/travis/AlbanAndrieu/ansible-jenkins-swarm.svg?style=flat)](http://travis-ci.org/AlbanAndrieu/ansible-jenkins-swarm) [![Branch](http://img.shields.io/github/tag/AlbanAndrieu/ansible-jenkins-swarm.svg?style=flat-square)](https://github.com/AlbanAndrieu/ansible-jenkins-swarm/tree/master) [![Donate](https://img.shields.io/gratipay/AlbanAndrieu.svg?style=flat)](https://www.gratipay.com/AlbanAndrieu)  [![Ansible Galaxy](http://img.shields.io/badge/galaxy-AlbanAndrieu.jenkins-swarm-660198.svg?style=flat)](https://galaxy.ansible.com/list#/roles/2000) [![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg?style=flat)](#)

Ensures that jenkins swarm is properly installed (using `apt`) and configured for a jenkins slave to be connected to the master

### Installation

This role requires at least Ansible `v1.6.3`. To install it, run:

    ansible-galaxy install AlbanAndrieu.jenkins-swarm



### Role variables

List of default variables available in the inventory:

```yaml
    ---
    jenkins_swarm_enabled: yes                       # Enable module
    jenkins_swarm_client_version: 1.9                # Swarm client version
    
    jenkins_name: jenkins
    jenkins_user: jenkins
    jenkins_group: jenkins
    jenkins_shell: "/bin/false"
    jenkins_home_dir: /var/lib/jenkins
    jenkins_url: https://home.nabla.mobi/jenkins
    jenkins_slave_name: swarm-{{ ansible_hostname }}
    #prompted jenkins_username: tbd
    #prompted jenkins_password: tbd
    
    docker_files_generated_directory: "./"
    docker_files_enable: no
    docker_volume_directory                  : "/var/log/jenkins"
    docker_working_directory                 : "/home/vagrant"
    docker_image_name                        : "nabla/ansible-jenkins-swarm"
```


### Detailed usage guide

Describe how to use in more detail...


### Authors and license

`jenkins-swarm` role was written by:
- [Alban Andrieu](fr.linkedin.com/in/nabla/) | [e-mail](mailto:alban.andrieu@free.fr) | [Twitter](https://twitter.com/AlbanAndrieu) | [GitHub](https://github.com/AlbanAndrieu)
- License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/AlbanAndrieu/ansible-jenkins-swarm/issues>)!

***

README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).

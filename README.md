ansible-docker-install
=====================

This role automates the process of installing Docker and Docker Compose on CentOS 7.

Role Variables
--------------

Modify the variables in vars/main.yml to suit your environment.

Example Playbook
----------------

Create an inventory file similar below:

    # vi inventory

    [server]
    docker.example.com ansible_host=192.168.122.85

Create playbook similar below:

    # vi site.yml

    --- 
    - hosts: server
      roles:
        - jancubillan.ansible_docker_install

Then run as follows:

    # ansible-playbook -i inventory site.yml

License
-------

MIT License

Author Information
------------------

Author: Jan Cubillan<br/>
GitHub: https://github.com/jancubillan<br/>
Ansible Galaxy: https://galaxy.ansible.com/jancubillan

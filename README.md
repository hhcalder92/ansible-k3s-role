K3s role 
=========

Sets up k3s on arm or x86 systems

Role Variables
--------------

 in defaults:
 
 in vars: 
 
Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: k3s_cluster
      become: yes
      roles:
        - role: k3s-role
        
Just nodes,

    - hosts: k3s_nods 
      become: yes
      vars: k3s_type: node
      roles:
        - role: k3s-role
        

License
-------

BSD

Inspiration
------------------

https://github.com/rancher/k3s-ansible
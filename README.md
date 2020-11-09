Role Name
=========

Spaghettio's. There's a more elegant way to handle filters and logic... 

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

defaults/main.yml:
* component: prometheus|node_exporter 

vars/main.yml:
Majority of these setting should remain static unless Prometheus changes repo naming conventions and structuring.
* base_dir: /tmp

vars/<component>.yml:
* component_version: specify the release you want to install

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, component: node_exporter }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

IT-Service "Adminka" App
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

path: "/home/core/itservice"
stream_virtual_host: "stream.it-premium.local"
stream_api: "http://stream.it-premium.local"
web_virtual_host: "beta.it-premium.com.ua"
mysql_root_password: 
sphinx_env: "production"
build_env: stage

sendgrid_username: 
sendgrid_password: 

secret_key_base: 

redis_url: redis://redis:6379
redis_host: redis

database_url: 
mysql_database: 
mysql_user: 
mysql_password: 
mysql_host: db

rails_env: production
rack_env: production
rails_serve_static_files: true

slack_notification: false
email_notification: false

slack_webhook_url: 
slack_webhook_channel: 

Dependencies
------------
Depends on mprokopov.nginx-proxy-certbot

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

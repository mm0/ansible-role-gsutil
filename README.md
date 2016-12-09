Ansible Role: gsutil
===================

[![Build Status](https://travis-ci.org/mm0/ansible-role-gsutil.svg?branch=master)](https://travis-ci.org/mm0/ansible-role-gsutil)

Install and setup gsutil with Ansible

Role Variables
---------------

Available variables are listed below, there are no defaults:

```yml
  gs_oauth2_refresh_token: 
```

Requirements
---------------

- Sudo access


Dependencies
---------------

None 


Example Playbook
---

```yml
 - hosts: all
   roles:
     - role: gsutil
       gsutil_users_config:
          - user: myuser
            group: mysuergroup # optional use user by default
            vars: 
              - gs_oauth2_refresh_token: "INSERT_YOUR_OAUTH2_REFRESH_TOKEN"
```

License
---------------

BSD-2

Author Information
------------------

[Matt Margolin](mailto:matt.margolin@gmail.com)

[mm0](https://github.com/mm0) on github
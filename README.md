ansible-role-create-dot-env-file
=========

Creates .env file from a template and places it in the correct directory

Requirements
------------
When you use this role, it expects a file in the template folder called `dot_env.j2`, you can customize the name of this template as described in the role variables below.

Role Variables
--------------

Check the file [defaults/main.yml](./defaults/main.yml) for details.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

Milad Kawas. @miladkawas

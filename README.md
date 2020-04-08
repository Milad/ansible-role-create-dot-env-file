ansible-role-create-dot-env-file
=========

Creates .env file from a template and places it in the correct directory

Requirements
------------
When you use this role, it expects a file in the template folder called `dot_env.j2`, you can customize the name of this template as described in the role variables below.

Role Variables
--------------

One variable is required only `dot_env_directory`.

```yaml
# The directory where the .env file is going to be saved. REQUIRED.
dot_env_directory: ""

# Group, owner and mode of the directory "dot_env_directory"
dot_env_directory_group: "www-data"
dot_env_directory_owner: "www-data"
dot_env_directory_mode: "0755"

# Whether to make sure the containing directory exists or not
dot_env_confirm_directory_exists: yes

# Source template of the .env file
dot_env_file_template: "dot_env.j2"

# Group, owner and mode of the .env file
dot_env_file_group: "www-data"
dot_env_file_owner: "www-data"
dot_env_file_mode: "0644"
```

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

# Demo service: Service1

Part of a demo of the Runner framework.

## Usage

### Demo files

The following files need to be changed to suit your environment:

- "env/envvars_demo"

    Contains the Ansible configuration variables for the service.

- "env/ssh_key_demo"
  
    Contains the SSH Private key for the service.

- "inventory/001_controllers_demo"

    Simple inventory file for the service. Store group and host variables in the inventory/group_vars and inventory/host_vars directories.

- "inventory/002_managed_demo"

    Simple inventory file for the service. Store group and host variables in the inventory/group_vars and inventory/host_vars directories.

### Group variables

The following group variables define which roles will be applied to the service. Set them in inventory/group_vars/controllers.yml file:

    ---
    git_roles:
      - name: role_test
        repo: https://github.com/Get-Tony/role_test
        version: main

### Create host_vars

Set the following variables in inventory/host_vars/localhost.yml file:

    ---
    ansible_python_interpreter: /usr/bin/python3
    ansible_connection: local

## License

This project is licensed under the MIT License.

## Author

This project was created by [Anthony Pagan](https://github.com/get-tony).

## Warning

This project is still in development and should not be used without proper testing.

Use at your own risk.

# Demo service: Service1

Part of a demo of the Runner framework.

## Usage

### Demo files

All '*_demo*' files need to be read, verified and renamed before use.

### Group variables

Set the following variables inventory/group_vars/controllers.yml file:

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

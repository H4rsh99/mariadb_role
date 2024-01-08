# MariaDB Ansible Role

This a Role to setup mariadb in your window server

## Requirements

-Ansible 
-Winrm Configured in your window server
-Port 5985 for winrm http traffic

## Role Variables

### User-settable variables:

- `mariadb_install_folder`: Path to the installation folder.
- `mariadb_installer_url`: URL for downloading the MariaDB installer.
- `mariadb_version`: Version of MariaDB to install.
- `mariadb_service_name`: Name of the MariaDB service.
- `mariadb_binary_path`: Path to the MariaDB binary.
- `mariadb_display_name`: Display name for the MariaDB service.
- `mariadb_startup_type`: Startup type for the MariaDB service.

## Dependencies

List any dependencies on other Ansible roles hosted on Galaxy or any specific requirements needed for successful execution.

## Example Playbook

An example playbook to demonstrate the usage of this role:

```yaml
- hosts: win
  roles:
    - mariadb_role

### Execution
To execute the role, use the following command:

"ansible-playbook -i tests/inventory tests/test.yml"

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

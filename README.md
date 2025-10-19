# Ansible Role: Git

[![CI](https://github.com/pluggero/ansible-role-git/actions/workflows/ci.yml/badge.svg)](https://github.com/pluggero/ansible-role-git/actions/workflows/ci.yml) [![Ansible Galaxy downloads](https://img.shields.io/ansible/role/d/pluggero/git?label=Galaxy%20downloads&logo=ansible&color=%23096598)](https://galaxy.ansible.com/ui/standalone/roles/pluggero/git)

An Ansible Role that installs and configures Git with secure defaults.

## Requirements

None.

## Role Variables

```yaml
git_install_method: "package"
```

The method used to install git can be defined in the variable `git_install_method`.
The following methods are available:

- `package`: Installs git from the package manager of the distribution
  - **NOTE**: This method installs the latest version available in the package manager and not the version defined in `git_version`.


## Example Playbook

### Basic Usage

```yaml
- hosts: all
  roles:
    - pluggero.git
```

## Dependencies

None.

## License

MIT / BSD

## Author Information

This role was created in 2025 by Robin Plugge.

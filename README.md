Role Name
=========

Install neovim

Requirements
------------

No requirements

Role Variables
--------------

```yaml
# Specify neovim version
# 0.3 -> 0.3.*: Install the newest version of neovim 0.3.x
# 0.3.1 -> 0.3.1: Install 0.3.1
# * -> *: Install latest version of repository
# Default is '*'.
neovim_version: "*"

# Choose repository from `stable` or `unstable`.
# If choose stable, add ppa:neovim/stable apt repository.
neovim_repository_channel: stable
```

Dependencies
------------

No dependencies

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - name: pddg.neovim
      vars:
        neovim_version: 0.3
        neovim_repository_channel: stable
```

License
-------

MIT

Author Information
------------------

[pddg](https://github.com/pddg/)
  - Web: [poyo.info](https://www.poyo.info/)



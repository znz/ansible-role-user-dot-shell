# Ansible role for `dot-shell` of user

- Setup [dot-shell](https://github.com/znz/dot-shell)

## Requirements

- Debian
- Ubuntu

## Role Variables

- `dot_shell_home_dir`: path to user's home directory
- `dot_shell_ghq_root`: path to [ghq](https://github.com/motemen/ghq) root
- `git_update`: `update` option of [git module](http://docs.ansible.com/git_module.html)
- `git_depth`: `depth` option of [git module](http://docs.ansible.com/git_module.html)
- `user_name`: argument of `git config --global user.name`
- `user_email`: argument of `git config --global user.email`

## Dependencies

None.

## Example Playbook

Normal usage:

    ---
    - hosts: all
      become: no
      roles:
      - znz.user-dot-shell

## Example requirements.yml

    - src: https://github.com/znz/ansible-role-user-dot-shell
      version: master
      name: znz.user-dot-shell

## License

MIT License

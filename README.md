# ansible-role-dotfiles

An ansible role to install my preferred dotfile settings.

## Requirements

Git on the client you are running this.

## Role Variables

| Variable | Default Value | Description|
| -- | -- | -- |
| dotfiles_repo | `https://github.com/chrisvanmeer/dotfiles.git` | The repository that holds the dotfiles. |
| dotfiles_repo_version| `main` | Defaults to new name convention. |
| dotfiles_repo_accept_hostkey | `false` | Accept repo hostkey if not present.
| dotfiles_repo_local_destination | `~/Documents/dotfiles` | Location where the repository is cloned.
| dotfiles_home | `~` | Defaults to current user home directory. |
| dotfiles_vim_colors_path | `.vim/colors` | Path to the .vim colors directory. |

## Dependencies

No dependencies.

## Installation

Install this role with the following command:

```
ansible-galaxy install chrisvanmeer.dotfiles
```

## Example Playbook

```
- hosts: server

  roles:
    - role: chrisvanmeer.dotfiles
```

## License

MIT

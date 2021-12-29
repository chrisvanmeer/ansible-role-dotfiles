# ansible-role-hashicorp

An ansible role to install my preferred dotfile settings.

## Requirements

No special requirements.

## Role Variables

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th width="150px">Default Value</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr valign="top">
      <td>dotfiles_home_path</td>
      <td><code>~</code></td>
      <td>Change this if you want this installed to a different user's directory. Defaults to current user directory.</td>
    </td>
  </tbody>
</table>

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

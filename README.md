VS Code
=========

A quick way to install VS Code using the Microsoft recommended method.

Requirements
------------

None

Role Variables
--------------

VS Code will install by default. If you want the repository and the insiders build only set this to false.
  vscode_install: true

To install VS Code insiders build set this to true.
  vscode_insiders_install: true

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

### Simple Installation

```
- hosts: servers
  roles:
      - ngetchell.vscode
```

### Installing Insiders

```
- hosts: servers
  roles:
    - {
        role: ngetchell.vscode,
        vscode_install: true,
        vscode_insiders_install: true
      }
```
License
-------

MIT

Author Information
------------------

Follow me on Twitter [@getch3028](https://twitter.com/getch3028) or at my PowerShell [blog](https://powershell.getchell.org).

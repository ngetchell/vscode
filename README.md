VS Code
=========

A quick way to install VS Code using the Microsoft recommended method.

Requirements
------------

None

Role Variables
--------------

VS Code will install by default. If you want the repository and the insiders build only set this to false.

```yaml
vscode_install: true
```

To install VS Code insiders build set this to true.

```yaml
vscode_insiders_install: true
```

Dependencies
------------

None

Example Playbook
----------------

```yaml
# role using defaults
- hosts: servers
  roles:
    - ngetchell.vscode

# role with variables
- hosts: servers
  roles:
    - role: ngetchell.vscode
      vars:
        vscode_install: true
        vscode_insiders_install: true

# role with extensions
---
- hosts: localhost
  roles:
    - ngetchell.vscode
  vars: 
    vscode_extension: 
      - ms-python.python
      - ms-vscode.powershell
      - ms-vscode.azurecli
```

License
-------

MIT

Author Information
------------------

Follow me on Twitter [@getch3028](https://twitter.com/getch3028) or at my PowerShell [blog](https://powershell.getchell.org).

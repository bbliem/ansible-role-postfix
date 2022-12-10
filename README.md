# ansible-role-postfix

Ansible role for Postfix on Debian and similar systems (e.g., Ubuntu)

## Variables

- `postfix_alias_root` [required]: Local user that should receive mail instead of the root user
- `postfix_myhostname` [required]: Example: `foo.example.com`
- `postfix_myorigin` [required]: Example: `example.com`
- `postfix_virtual_aliases` [required]: List of aliases such as `"@example.com bar@example.net"`

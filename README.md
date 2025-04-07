# ansible-role-postfix

Ansible role for Postfix on Debian and similar systems (e.g., Ubuntu)

## Variables

- `postfix_alias_root` [required]: Local user that should receive mail instead of the root user
- `postfix_myhostname` [required]: Example: `foo.example.com`
- `postfix_myorigin` [required]: Example: `example.com`
- `postfix_virtual_aliases` [required]: List of aliases such as `"@example.com bar@example.net"`
- `postfix_virtual_alias_domains` [optional]: Example: `example.net`. Use this, e.g., when you have more than one domain in `postfix_virtual_aliases`. Any domains there other than myorigin need to be added to `postfix_virtual_alias_domains` explicitly, otherwise Postfix won't accept mail for those domains.

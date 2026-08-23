# Security Policy

## Scope

This repository is an educational incident-response lab. All incidents, request IDs, customer-like identifiers, logs and datasets committed to the repository must be synthetic and must not originate from production systems.

## Secret handling

- Never commit API tokens, passwords, authentication cookies, recovery codes, private keys or production connection strings.
- Store local configuration in `.env` or another ignored local file.
- Use placeholders such as `<API_TOKEN>` in documentation and examples.
- Treat logs copied from real systems as sensitive even when they appear harmless.
- Rotate any credential immediately if it is accidentally committed; deleting the file in a later commit does not remove it from Git history.

## Reporting

If sensitive information is discovered in this repository, remove it from active content, rotate/revoke the affected credential, and purge it from Git history before considering the incident resolved.

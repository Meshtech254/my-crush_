# Security and privacy

This is a static frontend project. It has no backend, database, authentication, or built-in secret storage.

## Everything public is visible

Anything placed in `index.html`, JavaScript, CSS, or an asset file is sent to visitors and can be inspected. If the project is in a public repository, others can also read and download every committed file and its public history.

Never add:

- Passwords, tokens, API keys, or `.env` contents
- Private phone numbers or email addresses
- Real home, school, or work addresses
- Private conversations, photos, or identifying details without consent
- Any information that could put someone at risk

Removing sensitive text from the visible page does not make it secret if it still exists in the HTML, JavaScript, Git history, or repository assets. If a secret is committed accidentally, revoke or rotate it immediately and remove it from the repository history before publishing again.

## Reporting a problem

For a harmless bug, open a GitHub issue at **(https://github.com/Meshtech254/my-crush_)**. For a sensitive security or privacy concern, contact **254738641078** instead of posting the details publicly.

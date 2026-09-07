# Pull request style

Codex Drafter is the final publishing layer for pull requests created through its MCP tool.

## Rules

- Pull requests are drafts by default unless the caller explicitly requests otherwise.
- The caller supplies the substantive title and body; the server should not silently rewrite their meaning.
- Do not put references to Codex or AI in the PR title.
- Preserve the caller's PR body and append the authorship disclosure as the final block.
- The disclosure is always collapsed inside `<details>`.
- When `CODEX_BANNER_URL` is configured, the banner itself is clickable and links to `CODEX_BANNER_LINK`.
- If the banner URL is unavailable, use a linked text credit rather than a broken image.

The point of keeping these rules in the server is that Codex does not need to remember them separately in every repository.

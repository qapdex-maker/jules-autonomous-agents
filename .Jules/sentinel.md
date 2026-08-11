# Sentinel <span role="img" aria-label="shield">🛡️</span> Journal

## 2026-07-09 - Prompt Injection Safety Guardrails

**Vulnerability:** AI agents treating untrusted external content or user data
as instructions rather than raw data (prompt injection / indirect prompt
injection).

**Learning:** In a repository containing AI agent prompts, prompt injection is
a critical security vulnerability where untrusted inputs can lead to
unauthorized actions.

**Prevention:** Always include explicit boundaries and constraints to treat
untrusted inputs purely as raw data, never as directions.

## 2026-07-10 - Sibling Directory Traversal Bypasses

**Vulnerability:** Path validation checks like startsWith on a target path and
safe directory path are vulnerable to sibling directory traversal bypasses.

**Learning:** If the safe directory is "/safe" and target is
"/safe-sibling/file", target.startsWith(safe) is true, bypassing the check.

**Prevention:** Append path.sep to the resolved safe directory path before
validating that the target starts with the safe directory path.

## 2026-07-11 - Prompt Injection XML Tag Breakout

**Vulnerability:** Prompt injection via custom tag closing/escaping. If an
agent uses XML tags like `<user_text>` to encapsulate untrusted user input, an
attacker can include `</user_text>` in their input to break out of the
encapsulation and inject instructions.

**Learning:** Simple XML-tag encapsulation is vulnerable to escape sequences
analogous to HTML/SQL injection, allowing attackers to inject malicious
directions.

**Prevention:** Always sanitize untrusted input by stripping or escaping the
encapsulated XML closing tags using a case-insensitive regex (e.g.,
`replace(/<\/user_text>/gi, '')`) before interpolating it into the prompt to
prevent case-variant breakout attacks.

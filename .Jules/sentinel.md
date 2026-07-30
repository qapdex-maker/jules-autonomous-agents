# Sentinel <span role="img" aria-label="shield">🛡️</span> Journal

## 2026-07-09 - Prompt Injection Safety Guardrails

**Learning:** In a repository containing AI agent prompts, prompt injection
(and indirect prompt injection) is a critical security vulnerability. If
agents treat untrusted external content or user data as instructions rather
than raw data, it can lead to unauthorized actions.

**Action:** Enhance the Sentinel security agent's scanning guidelines to
include detection of prompt injection risks and untrusted input safety checks.

## 2026-07-10 - Sibling Directory Traversal Bypasses

**Vulnerability:** Path validation checks like startsWith on a target path and
safe directory path are vulnerable to sibling directory traversal bypasses.

**Learning:** If the safe directory is "/safe" and target is
"/safe-sibling/file", target.startsWith(safe) is true, bypassing the check.

**Prevention:** Append path.sep to the resolved safe directory path before
validating that the target starts with the safe directory path.

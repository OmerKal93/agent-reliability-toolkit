# agent-lint

Local-first static analyzer for AI agent reliability and security anti-patterns — unbounded agent loops (**AR001**), missing timeouts (**AR003**), and unbounded retries (**AR014**).
Broader suite ideas in the repo PLAN are not shipped in this package.

```bash
# not on PyPI yet — from this repo:
cd packages/agent-lint && uv sync --dev
uv run agent-lint scan .
```

Runs entirely offline: no account, no API key, no network access, `network: deny` by default.
Findings are deterministic (AST-based), not model-generated.

**Status:** early development. See the
[project root](https://github.com/OmerKal93/agent-reliability-toolkit) for the full plan
(`PLAN.md`, `PLAN-PRS.md`, `EXECUTION.md`) and current progress.

Licensed under Apache-2.0.

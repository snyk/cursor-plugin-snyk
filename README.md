# Snyk for Cursor

**Innovate with AI. Securely.**

Embed [Snyk](https://snyk.io/platform/) directly into Cursor — so AI-generated code is **secure at inception**, not patched after the fact.

---

## Is this for me?

**Yes**, if any of these apply:

- You use **Cursor** and want every line of AI-assisted code scanned, fixed, and governed automatically.
- You're already a Snyk customer and want a fast, concrete way to **apply Secure at Inception** to agentic development without writing custom integrations.
- You're evaluating how to keep AI velocity from outrunning your security posture.

If you haven't heard the term *Secure at Inception*, the [What is Secure at Inception?](#what-is-secure-at-inception) section below is the 60-second primer.

---

## What you get

| Capability | What it does | When it fires |
|---|---|---|
| **Secure at Inception guardrails** | Auto-scan AI-generated code and new dependencies for vulnerabilities the moment they're written. | Continuously, as Cursor writes code. |
| **Remediation commands** | Find, fix, validate, and PR security issues in one guided flow (`/snyk-fix`, `/snyk-batch-fix`). | On demand from you or the agent. |
| **Dependency health check** | Before adding a package, evaluate its maintenance health, popularity, and community standing — not just known CVEs. | On demand, when considering a new dependency. |
| **Snyk MCP integration** | Wires Snyk's CLI and scanners into Cursor via the [Snyk MCP server](https://docs.snyk.io/integrations/snyk-studio-agentic-integrations/getting-started-with-snyk-studio). | Automatically, once installed. |

---

## What is Secure at Inception?

AI coding assistants generate code at machine speed. Traditional security tooling — scanning at PR time, in CI, or at deploy — runs *after* the code is written and reviewed, which means risky code has already shaped the design, the tests, and the developer's mental model by the time anyone sees a finding.

**Secure at Inception** flips that: security checks run **at the moment of generation**, inside the assistant's loop, so vulnerabilities are caught and fixed before they ever land in a commit. It's Snyk's approach to keeping AI-driven development [fast *and* safe](https://snyk.io/product/studio/) — preventing new AI-generated risk while remediating existing security debt at the same speed your team is now writing code.

This plugin is the implementation. Snyk Studio is the platform.

---

## Quick start

**1. Prerequisites**

- A Snyk account — after installation, run `snyk auth` or set `SNYK_TOKEN` so the plugin can scan.

**2. Install**

Install from the [Cursor Plugin Marketplace](https://cursor.com/plugins) — search for **Snyk**.

**3. Authenticate**

Authenticate the Snyk CLI so the installed plugin can scan:

```bash
snyk auth
```

Or set the `SNYK_TOKEN` environment variable from your [Snyk account](https://app.snyk.io/account) for non-interactive environments (CI, containers, shared workstations).

**4. Try it**

Ask Cursor to write code that touches a database, a network call, or a new dependency. You should see Snyk run automatically. Then try `/snyk-fix` on an existing project to see remediation in action.

---

## Customize and extend

These are starting points, not rigid templates. Common customizations:

- Adjust scan thresholds and severity gates
- Add or remove workflow phases in remediation commands
- Compose multiple capabilities into a workflow tuned to your team

Snyk Studio is built on an open, partner-first, tool-agnostic foundation — this plugin follows the same philosophy.

---

## Learn more

- [Snyk Studio product page](https://snyk.io/product/studio/) — the product this plugin integrates with
- [Snyk Platform](https://snyk.io/platform/) — the broader AI-native security platform
- [Snyk Studio documentation](https://docs.snyk.io/integrations/snyk-studio-agentic-integrations/getting-started-with-snyk-studio) — setup, MCP server, and reference material

---

## Need help?

Reach out to your Snyk account team, or open an issue in this repository.

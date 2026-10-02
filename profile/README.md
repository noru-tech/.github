# Noru

Open-source tools for compliance you can verify: change control for AI coding agents, privacy data
maps and personal-data flows from source code, and GRC checks that run in your repository and CI.

## Open-source tools

| Tool | What it is | Install |
| --- | --- | --- |
| [agent-change-control](https://github.com/noru-tech/agent-change-control) (`acc`) | Deterministic change control for code written by AI coding agents. Checks each change for independent human approval and emits SARIF and in-toto statements. | `brew install noru-tech/tap/acc` |
| [privacy-flow](https://github.com/noru-tech/privacy-flow) (`piiflow`) | Finds where personal data goes in TypeScript, JavaScript and Python: logs, third-party SDKs, LLM providers and outbound HTTP. Offline and deterministic, every hop cited, with SARIF and Fides output. | `brew install noru-tech/tap/piiflow` |
| [fideslang-tools](https://github.com/noru-tech/fideslang-tools) (`fl`) | Rust CLI for Fideslang privacy taxonomies and Fides manifests. Browse, validate, merge, convert and graph data maps offline. | `brew install noru-tech/tap/fl` |
| [noru-grc-engineering](https://github.com/noru-tech/noru-grc-engineering) | Last-mile GRC engineering plugins for Claude Code and Codex: AI inventory, privacy data maps, infrastructure checks and change control, recorded in Noru. | `/plugin marketplace add noru-tech/noru-grc-engineering` |
| [compliance-assistant](https://github.com/noru-tech/compliance-assistant) | Claude Code and Codex plugin that guides SOC 2, ISO 27001 and other framework work through Noru's MCP server. For Noru customers. | `/plugin marketplace add noru-tech/compliance-assistant` |

GitHub Actions, each usable on its own:

| Action | What it does on a pull request |
| --- | --- |
| [`noru-tech/agent-change-control`](https://github.com/noru-tech/agent-change-control/blob/main/docs/github-action.md) | Flags an agent-written change until a human independent of its author or operator approves the current head, with SARIF output. |
| [`noru-tech/privacy-flow`](https://github.com/noru-tech/privacy-flow/blob/main/docs/github-action.md) | Reports the personal-data flows a pull request introduces as code-scanning alerts. |
| [`noru-tech/noru-ci-action`](https://github.com/noru-tech/noru-ci-action) | Re-checks a committed Noru compliance manifest and fails when it drifts from the code. Offline by default. |
| [`noru-tech/noru-review-action`](https://github.com/noru-tech/noru-review-action) | Routes the diff to the affected Noru compliance checks and reports findings. Read-only. |
| [`noru-tech/noru-enforce-action`](https://github.com/noru-tech/noru-enforce-action) | Makes committed compliance records a merge condition across every configured piece. |

To see `acc` on real pull requests before installing anything, open
[agent-change-control-demo](https://github.com/noru-tech/agent-change-control-demo): ten pull
requests that stay open, each showing one verdict.

Every release binary carries a GitHub artifact attestation and a checksum, and the
[Homebrew tap](https://github.com/noru-tech/homebrew-tap) installs those binaries pinned by
SHA-256. To check a download yourself: `gh attestation verify <archive> --repo noru-tech/<repo>`.

## About Noru

[Noru](https://noru.tech) is a continuous compliance platform. It collects evidence, monitors
controls and keeps teams audit-ready across SOC 2, ISO 27001, GDPR, NIS2 and other frameworks by
syncing the tools they already use (AWS, GCP, Azure, GitHub, GitLab, Slack, Google Workspace and
more). The tools above work without a Noru account unless their description says otherwise.

## Contributing and security

These policies apply to every repository in the organization unless a repository has its own.

- [How to contribute](https://github.com/noru-tech/.github/blob/main/CONTRIBUTING.md)
- [Reporting a vulnerability](https://github.com/noru-tech/.github/blob/main/SECURITY.md): use
  the repository's **Security > Report a vulnerability** form for private reporting
- [Getting help](https://github.com/noru-tech/.github/blob/main/SUPPORT.md)
- [Code of conduct](https://github.com/noru-tech/.github/blob/main/CODE_OF_CONDUCT.md)

# Solaris Dev Shop for Claude

61 specialist workflows, a chief of staff and executable local helpers, published
by Solaris Technologies. Version 0.68.0 carries the reviewed security corrections in the
[Solaris Dev Shop 0.68 candidate](https://github.com/Shaisolaris/solaris-dev-shop/tree/c7c9b395795f488dd3c48122ff916970438b67e6).
This separate Claude distribution keeps the complete roster while avoiding the
universal repository's copies for other platforms.

## Installation and status

This is the source prepared for a Claude plugin-directory submission. It is not
an approved directory listing. The plugin folder is the repository root, and the
Claude manifest is `.claude-plugin/plugin.json`. For an existing Claude Code
marketplace installation, use the public universal distribution:

```text
/plugin marketplace add Shaisolaris/solaris-dev-shop-plugins
/plugin install solaris-dev-shop@solaris-technologies
```

The directory listing will use this repository after its independent checks and
Anthropic review. A paid account enables submission; it does not grant approval.

## Try a workflow

Ask Claude to use one of the named Solaris skills. For example:

1. "Use the Solaris chief of staff to route a request to review this code. Return
   a bounded assignment and do not claim the review has already happened."
2. "Use the Solaris code reviewer to inspect this public example diff. Report
   concrete defects with file references and distinguish untested assumptions."
3. "Use the Solaris delivery lead with synthetic evidence to check a milestone's
   acceptance conditions and identify missing proof."

The skill wrappers load their bundled canonical workflows. The
[capability guide](docs/capabilities.md) describes runnable local helper examples;
the [upstream README](SOURCE-README.md) documents the full roster. Helpers run only
when explicitly invoked through the host's available tools. Their prerequisites
and input/output locations are documented with each helper. Python helpers need
the Python version and dependencies stated by that workflow; native applications
and optional third-party services require their own installation and access.

## Execution, services and data

The Claude manifest configures no MCP servers, hooks or background schedules. It
does not install tools, create accounts, grant file access or supply credentials.
Claude and its tools determine access and approval behavior. Some selected
workflows can run local commands, read project files, write local reports or
SQLite journals, start explicit demonstration services, fetch references, or use
the external tools described in their instructions. There is no Solaris backend
that automatically receives those inputs or outputs.

The complete bundle includes optional image-generation, voice/audio, video,
payments, infrastructure and other professional workflows. These require their
respective tools and permissions; the presence of instructions does not create
an integration or authorize a transaction. Use synthetic data for demonstrations
and review remote destinations before sending real data. Any external service's
authentication, charges and privacy policy remain separate. Anthropic eligibility
for the complete bundle, including media workflows, is subject to its review.

[Plugin data handling](DATA-HANDLING.md) describes local storage, retention and
host/model processing. The publisher's
[website privacy policy](https://www.solaristek.com/privacy-policy/) has its own
website scope. Do not send secrets or private customer data to public support.

## Scope and provenance

The roster is 61 specialists plus one coordinator. Source/runtime improvements
were recorded for 37 roles in the original programme; roster presence is not
proof that every role gained new executable behavior. Native discovery and local
helper checks are separate from a live model's skill activation and production
security or quality certification. Host support also differs across Claude apps.

`SOLARIS-BUILD-SOURCE.json` records all 1,199 canonical file hashes. The additional
`CLAUDE-DISTRIBUTION.json` identifies this provider-facing packaging operation.
The bundled 740,394-byte `google-fonts.csv` is readable design-reference data;
it is retained intact and may require a directory reviewer because it exceeds
the directory's 256 KiB non-image/font-file threshold. It is not an executable.

Support: [GitHub issues](https://github.com/Shaisolaris/solaris-dev-shop-claude/issues)
or shehryar@solaristek.com. Published under the upstream [MIT license](LICENSE),
with the bundled notices and attribution retained.

Canonical GitHub CI is retained as inert source data under `source-config/.github`; this distribution runs its own exact packaging validation. The 0.65 candidate is not a provider approval.

Loading this package does not start Docker, MCP/database services, an updater or learning rewrites. Optional setup is task-scoped. The managed CLI installer uses only offline router checks; complete developer and release QA remain separate gates.

# Where this code lives

This repository is the standalone home of the `canli-fundamentals-mcp` package, published so the server can be
installed, scanned and reviewed on its own. It is imported from the `mcp-fundamentals/` directory of
[arhancanli/canlicapital](https://github.com/arhancanli/canlicapital/tree/main/mcp-fundamentals), which is
where changes are made and tested; this repository is updated from it.

Imported from canlicapital commit `4f517160563fa54482a49263344d3989004d4305` (tag `fundamentals-mcp-v0.6.0`).

- npm: https://www.npmjs.com/package/canli-fundamentals-mcp
- MCP Registry: `io.github.arhancanli/canli-fundamentals-mcp`
- Hosted endpoint (no install): https://canlicapital.com/mcp/fundamentals

The Claude Desktop bundle attached to each release is built by `.github/workflows/release.yml` from
the files committed at the release tag (`mcp-fundamentals/mcpb/build.sh` in canlicapital does the same), with
a signed build provenance attestation:

```bash
gh attestation verify canli-fundamentals.mcpb --repo arhancanli/canli-fundamentals-mcp
```

Files owned by this repository and kept across syncs: `.github/` (CI, CodeQL, OpenSSF Scorecard,
Dependabot, and the release workflow that builds, signs and attaches the Claude Desktop bundle),
`.gitignore`, `MIRROR.md`, `glama.json`, and the digest-pinned base image in `Dockerfile`.

The portable seven-tool server, guides and packed install run here on Node 20/22/24.
Supplied-input audit and expert-command tests that read the parent monorepository
run in canlicapital CI against these exact source bytes; they are retained in test/
and are not presented as standalone test results.

# Where this code lives

This repository is the standalone home of the `canli-fundamentals-mcp` package, published so the server can be
installed, scanned and reviewed on its own. It is imported from the `mcp-fundamentals/` directory of
[arhancanli/canlicapital](https://github.com/arhancanli/canlicapital/tree/main/mcp-fundamentals), which is
where changes are made and tested; this repository is updated from it.

Imported from canlicapital commit `4d40d90edb20bb86eae228e6c4b7762bacdd41fa`.

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

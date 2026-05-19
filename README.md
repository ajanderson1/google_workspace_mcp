# Google Workspace

MCP server providing natural language control over Google Workspace services (Gmail, Calendar, Drive, Docs, Sheets, Slides). Source code lives directly in this directory (the slug dir IS the submodule, which is the operator's fork of `taylorwilsdon/google_workspace_mcp`).

## Install

See `~/.conventions/conventions/mcps.md` for the install procedure. Default invocation runs the fork locally so fork patches apply:

```
cd mcps/google-workspace
uv run main.py
```

If you'd rather use the upstream PyPI release (which won't include fork patches):

```
uvx workspace-mcp
```

## Notes

- Source: `mcps/google-workspace/` (git submodule, slug dir is the submodule itself, operator's fork).
- Requires `GOOGLE_OAUTH_CLIENT_ID` and `GOOGLE_OAUTH_CLIENT_SECRET` env vars.
- `--tool-tier core` flag is recommended for a minimal footprint.

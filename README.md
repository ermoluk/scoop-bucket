# ermoluk/scoop-bucket

[![Tests](https://github.com/ermoluk/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/ermoluk/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/ermoluk/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/ermoluk/scoop-bucket/actions/workflows/excavator.yml)

A [Scoop](https://scoop.sh) bucket for
[mcp-warden](https://github.com/ermoluk/mcp-warden), a local-first credential
broker for the Model Context Protocol.

```pwsh
scoop bucket add ermoluk https://github.com/ermoluk/scoop-bucket
scoop install ermoluk/mcp-warden
```

The manifest installs the prebuilt Windows x86_64 release binary and checks it
against the release's SHA-256. Excavator picks up new releases through
`checkver` / `autoupdate`; mcp-warden itself never updates on its own. Update
with `scoop update mcp-warden`.

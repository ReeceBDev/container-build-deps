# container-build-deps

Pinned build assets published as GitHub release assets, for CI builds whose network egress is restricted to GitHub.

Every release asset is a pristine vendor distribution — nothing is rebuilt or modified. Each release's notes record the source URL, download date, and sha256; the consuming build verifies the digest before extracting.

## Releases

- [v1](https://github.com/ReeceBDev/container-build-deps/releases/tag/v1) — dotnet-sdk-10.0.401-linux-x64.tar.gz (Microsoft .NET SDK 10.0.401, linux-x64, downloaded from https://builds.dotnet.microsoft.com/dotnet/Sdk/10.0.401/dotnet-sdk-10.0.401-linux-x64.tar.gz on 2026-11-24), sha256 137268c8ad939c064ff1ee2a6fdf0899d8725377114ea012fbd1ad5fa2550418. Consumed by ReeceBDev/agentic-framework-2 (pipeline/Dockerfile).

## Adding an asset

Upload the untouched vendor distribution as a release asset, and record its source URL, download date, and sha256 in the release notes.

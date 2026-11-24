# container-build-deps

Pinned build assets served for the CI egress allowlist. The CI engine's
egress is pinned to GitHub + build package infrastructure
(/opt/vps-1-infra-repo/ops/ci-egress-lock.sh); its own law: "if a build needs
such material, serve it from GitHub". This repo is that GitHub shelf.

Each release asset records its provenance and sha256 in the release notes;
the consuming build verifies the digest before extracting. Assets are
pristine vendor distributions — nothing is rebuilt or modified.

## Releases

- v1 — dotnet-sdk-10.0.401-linux-x64.tar.gz (Microsoft 10.0.401, sha256
  137268c8ad939c064ff1ee2a6fdf0899d8725377114ea012fbd1ad5fa2550418),
  consumed by ReeceBDev/agentic-framework-2 pipeline/Dockerfile.

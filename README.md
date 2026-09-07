# linux-tools

Small reusable Linux shell tooling.

## Contents

| Path | Language | What it does | Effect |
|---|---|---|---|
| `shell/ubuntu-docker-install.sh` | bash | Installs Docker CE on Ubuntu Server (apt repository setup, engine, compose plugin) | **changes the host** (package installation) |
| `docs/legacy-README-linux-ubuntu-shell.md` | — | Original README | — |

## Prerequisites

Ubuntu Server with sudo; internet access to the Docker apt repository.

## Environment-specific configuration

None stored here. Site-specific compose files and NAS backup scripts from the previous
repositories are kept outside this repository.

## Credentials and safety

No credentials are stored in this repository. PowerShell scripts prompt (`Get-Credential`) or read
environment variables; Ansible playbooks expect an Ansible Vault (`--ask-vault-pass`) providing the
`vault_*` variables named in `group_vars`. Never commit vault files, Clixml exports or `.env` files
(see `.gitignore`). Run output (reports, CSV, logs) is generated content and is git-ignored; keep it
outside the repository.

## Provenance

Consolidated from previous local automation repositories during the 2026 LabOps repository
cleanup. This repository starts with a fresh history; earlier history is retained locally only.

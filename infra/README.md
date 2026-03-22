# infra — Personal Cloud Infrastructure

Terraform monorepo for personal AWS and Google Cloud management.

This repository manages cloud resources using a phased approach, starting with
a minimal skeleton and incrementally adding provider-specific configurations.

## Roadmap

- **Phase 1** (current): Repository skeleton — directory layout, shared configuration, and documentation. No cloud credentials required.
- **Phase 2**: AWS root modules — add provider configuration and AWS resources under `aws/`.
- **Phase 3**: GCP root modules — add provider configuration and Google Cloud resources under `gcp/`.

## Prerequisites

All tools below are required; configuration details will be added per phase.

- **Terraform** >= 1.7 — see `.terraform-version` for the pinned version
- **AWS CLI** — to be configured in Phase 2
- **gcloud CLI** — to be configured in Phase 3

> **Note:** No cloud credentials are needed for Phase 1. The directory structure
> and documentation are the only deliverables at this stage.

## Directory Layout

```
infra/
├── README.md                 # This file
├── .gitignore                # Terraform, OS, and editor exclusions
├── .terraform-version        # Pinned Terraform version
├── modules/                  # Reusable Terraform modules (added per phase)
├── aws/                      # AWS root modules (Phase 2)
└── gcp/                      # GCP root modules (Phase 3)
```

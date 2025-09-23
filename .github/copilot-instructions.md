# Copilot Instructions for AI Coding Agents

## Project Overview
This repository appears to be a backend or API documentation project, with a focus on ad-related workflows, user authentication, points, and rewards. The structure is organized by feature domains, each with its own YAML API specs and data models.

## Key Directories & Files
- `apis-doc/` — Main API documentation and configuration
  - `ads/` — Ad-related endpoints (like ad-like, ad-watch, ads-get)
  - `auth/` — Authentication endpoints (send_otp, update_profile, verify, etc.)
  - `data-structure/` — Core data models (ads, rewards, user)
  - `points/` — Points system endpoints (ad-watch, add-friends, redeem, etc.)
  - `rewards/` — Rewards endpoints (ad-watch, get, redeem)
- `ads-videos/` — Media assets for ads (SVG, MP4)
- `read-me` — (No README.md found; may be a placeholder or misnamed)

## Architecture & Patterns
- **API-First Design:** All endpoints and data models are defined in YAML under `apis-doc/`, suggesting a contract-driven or OpenAPI-like workflow.
- **Feature Modularity:** Each domain (ads, auth, points, rewards) is separated for clarity and maintainability.
- **YAML-Driven:** All API and data structure definitions are in YAML, not code. There is no evidence of implementation code in this repo.

## Developer Workflows
- **API Changes:** Edit or add YAML files in the relevant `apis-doc/` subdirectory. Keep data models in sync with endpoint definitions.
- **Media Updates:** Place new ad assets in `ads-videos/`.
- **No Build/Test Scripts:** No build, test, or CI/CD scripts are present. This repo is likely documentation/spec only.

## Project-Specific Conventions
- **Naming:** Use kebab-case for YAML files and directories.
- **Versioning:** No explicit versioning found; maintain backward compatibility manually.
- **Duplication:** Some files are suffixed with `copy` (e.g., `send_otp copy.yaml`), likely for drafts or alternate versions. Clean up when finalizing changes.

## Integration Points
- **External Consumers:** These YAML files are likely consumed by other services, code generators, or documentation tools. Ensure changes are communicated to downstream consumers.

## Examples
- To add a new ad endpoint: create a new YAML file in `apis-doc/ads/` and update related data models in `apis-doc/data-structure/`.
- To update user authentication: modify YAML in `apis-doc/auth/`.

## Recommendations for AI Agents
- Always keep data models and endpoint definitions in sync.
- Avoid breaking changes unless coordinated with all consumers.
- Document any new conventions in this file for future agents.

---
_Last updated: September 23, 2025_

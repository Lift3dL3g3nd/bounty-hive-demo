# Bounty-Hive GitHub Actions Demo

This repository demonstrates how Bounty-Hive governance can be integrated
into a CI/CD workflow using GitHub Actions.

The workflow simulates governance enforcement on security artifacts before
they are accepted into a repository or pipeline.

## Demo Workflow

When an artifact is pushed to this repository:

1. GitHub Actions workflow runs
2. The private Bounty-Hive engine is pulled
3. Governance policies are applied to the artifact
4. Lifecycle and policy invariants are enforced
5. A receipt and audit output are generated
6. The artifact is either admitted or rejected

## Repository Structure

demo_artifacts/   → Example artifacts to be governed
policies/         → Example governance policies
output/           → Governance results and receipts
.github/workflows → GitHub Actions workflow

## Purpose

This demo shows how governance and policy enforcement can be applied
to operational artifacts inside automated workflows and CI/CD pipelines.

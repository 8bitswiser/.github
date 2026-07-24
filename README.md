<img src="https://8bitswiser.com/8-bits-wiser.svg" alt="8 Bits Wiser logo" width="200"/>

Technology Consulting // AI/ML & Data Analytics // Website Development & SEO

🌎 [8bitswiser.com](https://8bitswiser.com/)

✉️ [Get in contact](mailto:contact@8bitswiser.com)

## Reusable workflows

The organization repository also owns two small workflow primitives:

- `validate-site.yml` installs from the lockfile, audits production
  dependencies, runs the caller's validation and optional browser smoke
  commands, and can upload a validated build.
- `deploy-worker.yml` downloads and verifies that build, optionally applies
  migrations, deploys with Wrangler, and proves the exact deployed version is
  receiving 100% of traffic.

Callers keep their own change detection, environment boundaries, cache purges,
multi-Worker ordering, and other repository-specific orchestration.

## What changed and why

<!-- One or two sentences. Link the issue or incident if there is one. -->

## How it was checked

- [ ] `kustomize build overlays/staging` and `kustomize build overlays/prod` both succeed
- [ ] Image tags are immutable Git SHAs (never `latest`)
- [ ] A prod change copies a tag that is already verified in staging
- [ ] No secret values in the diff (secrets come from External Secrets)

## Risk and rollback

<!-- What could break, and how to undo it (usually: revert this PR). -->

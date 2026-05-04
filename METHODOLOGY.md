# Methodology

1. Fetch the latest domain list from `email-disposable`.
2. Normalize and de-duplicate domains.
3. Join domains against Gatekeepr disposable-domain profiles.
4. Refresh missing MX snapshots within the configured daily budget.
5. Infer provider clusters from cleaned MX hostnames and resolved public MX IPs.
6. Write latest CSV/JSONL datasets and dated diff files.

Provider clusters are inferred from mail-routing infrastructure. They are not ownership assertions.

# Disposable Email Infrastructure

Public disposable email infrastructure data derived from the daily [email-disposable](https://github.com/gtkppr/email-disposable) domain list and Gatekeepr MX enrichment.

## Data

- `data/latest/domains.csv` and `domains.jsonl`: disposable domains with MX hosts, MX IPs, and provider cluster references.
- `data/latest/providers.csv` and `providers.jsonl`: provider clusters inferred from MX routing infrastructure.
- `data/latest/mx_hosts.csv`: MX hostnames seen across disposable domains.
- `data/latest/mx_ips.csv`: resolved public MX IP addresses seen across disposable domains.
- `data/latest/summary.json`: generation timestamp and aggregate counts.
- `data/diffs/YYYY-MM-DD/`: daily change files compared with the previous published `data/latest` snapshot.
- `data/schema/`: JSON Schema files for JSONL rows.
- `data/sources.json`: upstream source and enrichment provenance.

## Update Cadence

This repository is generated daily shortly after the `email-disposable` package is updated.

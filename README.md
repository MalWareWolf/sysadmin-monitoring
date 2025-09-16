# SysAdmin Monitoring — small, practical monitoring suite

**Purpose:** Small, reproducible monitoring stack for Windows & Linux servers. Includes collectors (PowerShell/Bash), Prometheus exporters config, Grafana dashboards, and alerting examples (Microsoft Teams + email).

> ⚠️ This project is for lab/testing and production-ready reference only — test in a controlled environment.

## Highlights
- PowerShell collector that gathers CPU, memory, disk, and Windows update status.
- Bash collector for Linux (proc/stat, df, memory, systemd services).
- Grafana dashboard JSON (Server Overview) for quick import.
- Example alert rule and Teams webhook script for notifications.

## Quick start
1. Copy a collector to your machine: `collectors/windows/collect-windows-metrics.ps1`.
2. Configure a Prometheus scrape job (see `exporters/sample-node-exporter-config.yml`).
3. Import Grafana dashboard: `grafana/dashboards/server-overview.json`.
4. Enable alerts: `alerts/alerting-rules.yml` and use `alerts/teams-alert.ps1` for Teams notifications.

## Legal / Use
For monitoring your own infrastructure only.

## Contribute
PRs welcome. See `docs/getting-started.md` for dev notes.

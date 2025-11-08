# grafana-observability-journey
Documenting my beginner-to-expert journey in DevOps observability using Grafana Alloy, Loki, and Grafana Cloud. This repo includes setup steps, configs, dashboards, and reflections as I learn to build telemetry pipelines, monitor Windows systems, and apply cloud-native monitoring.
# Grafana Observability Journey 🚀

This repository documents my hands-on learning and implementation of Grafana Alloy, Loki, and Grafana Cloud for Windows system monitoring. It reflects my progress in mastering DevOps observability tools and practices.

## 🎯 Goals
- Learn and deploy Grafana Alloy for telemetry collection
- Configure log processing and forwarding to Grafana Cloud
- Build dashboards for Windows system metrics and logs
- Troubleshoot integrations and validate observability pipelines
- Share insights and configs for community and employer visibility

## 🛠️ Tools Used
- Grafana Alloy
- Grafana Cloud (Loki, Dashboards)
- Windows 10
- Visual Studio Code
- GitHub for documentation

## 📅 Progress Timeline
| Date       | Milestone                                      |
|------------|------------------------------------------------|
| Nov 8, 2025| Installed Grafana Alloy on Windows             |
| Nov 8, 2025| Created `config.hcl` for Windows Event Logs    |
| Nov 8, 2025| Connected Alloy to Grafana Cloud (Loki)        |
| Nov 8, 2025| Validated log ingestion and dashboard setup    |
| Nov 9, 2025| Drafted GitHub repo to document journey        |


## 📌 Next Steps
- Add CPU, memory, and disk metrics via Prometheus scrape
- Create alert rules for log severity and system health
- Explore Observability as Code (versioned dashboards)
- Integrate with GitHub Actions for config validation

## 💼 Why This Matters
This repo demonstrates my practical experience in DevOps observability, telemetry collection, and cloud-native monitoring. It reflects my ability to troubleshoot, document, and deliver resilient monitoring solutions.





# 🧠 Reflection: Setting Up Grafana Alloy on Windows

## 🔧 What I Did
- Downloaded Grafana Alloy binary for Windows from GitHub Releases
- Created a `config.hcl` file to collect Windows Event Logs (Application, System, Security)
- Configured log parsing using `stage.json` to extract `levelText`, `source`, and `message`
- Connected Alloy to Grafana Cloud Loki using API token and tenant ID
- Ran Alloy via PowerShell and validated log ingestion in Grafana Explore

## ⚠️ Challenges Faced
- Initially downloaded the wrong `.deb` package meant for Linux
- Faced a 404 error when accessing Grafana docs for alerting setup
- Needed to troubleshoot missing metrics during the “Test Connection” phase

## ✅ What I Learned
- Grafana Alloy uses HCL for modular telemetry configuration
- Windows logs require careful parsing to extract meaningful fields
- Grafana Cloud’s Explore tab is essential for validating data flow
- GitHub is a powerful tool to document and share observability work

## 🎯 Next Steps
- Add Prometheus scrape config for CPU, memory, and disk metrics
- Build dashboards with panels for system health and log severity
- Create alert rules for error-level logs and high resource usage
- Version dashboards and configs in GitHub for Observability as Code

## 💼 Why This Matters
This setup demonstrates my ability to deploy and troubleshoot observability pipelines in a Windows environment using Grafana tools. It reflects my readiness for DevOps roles focused on monitoring, logging, and cloud-native infrastructure.

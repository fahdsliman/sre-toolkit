
SRE Toolkit

SRE Toolkit is a hands-on environment I built to learn and demonstrate core Site Reliability Engineering skills by building, monitoring, and automating real systems — not just reading about them.

This project simulates the tools and workflows used by SREs in production environments (e.g., fintech or payments systems). It’s designed for reliability practice, observability setup, and automation scripting.

---

Features

- **System Monitoring Agent (`sysmon.py`)**  
  Collects real-time CPU, memory, disk, and network usage using `psutil`. Outputs metrics as JSON logs and exposes them over HTTP in Prometheus format.

- **Alerting System (`alerter.py`)**  
  Watches resource metrics and triggers alerts via Slack or email when thresholds are exceeded (e.g., CPU > 80%, disk > 90%).

- **Prometheus Integration**  
  Built-in `/metrics` endpoint to scrape metrics. Can be visualized using Grafana dashboards.

- **Dockerized Environment**  
  Includes a `docker-compose.yml` to spin up:
  - `sysmon` service (Python monitoring agent)
  - `prometheus` (for scraping)
  - `grafana` (for visualization)

- **Logging & Observability**  
  Logs system performance to local files and exposes metrics suitable for real-time dashboards and alerting rules.

---

Tech Stack

| Component | Purpose | Tools Used |
|------------|----------|-------------|
| **Programming** | Scripting & automation | Python 3.11 |
| **Metrics** | System stats collection | psutil, prometheus_client |
| **Alerting** | Notification triggers | Slack Webhook / SMTP |
| **Containers** | Portable setup | Docker, Docker Compose |
| **Visualization** | Dashboards | Prometheus, Grafana |
| **OS** | Base environment | Linux / Ubuntu (or WSL2) |


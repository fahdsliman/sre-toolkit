SRE Toolkit — a reliability automation platform designed to simulate and manage production-grade systems. Includes Python-based observability agents, self-healing automation, chaos testing tools, alert routing, and Terraform-based infrastructure templates. Demonstrates expertise in monitoring, automation, and fault tolerance across containerized environments (Docker / Kubernetes / Prometheus / Grafana / Terraform).

sre-toolkit/
├── observability/
│   └── sysmon_agent/
│       ├── app.py
│       ├── Dockerfile
│       └── requirements.txt
├── reliability/
│   └── tx_checker/
│       ├── app.py
│       ├── Dockerfile
│       └── requirements.txt
├── infra/
│   ├── docker-compose.yml
│   └── prometheus.yml
├── oncall/
│   └── alert_router/
│       ├── app.py
│       └── requirements.txt
├── docs/
│   └── runbooks.md
├── .env.example
├── .gitignore
├── README.md
└── LICENSE

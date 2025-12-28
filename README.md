Linux / DevOps engineer | Amateur Radio & Big Data enthusiast | Exploring AI Agent (MCP) integrations

![Linux](https://img.shields.io/badge/Linux-Advanced-teal?style=flat-square)
![Bash](https://img.shields.io/badge/Bash-Advanced-teal?style=flat-square)
![Python](https://img.shields.io/badge/Python-Advanced-teal?style=flat-square)
![CSharp](https://img.shields.io/badge/CSharp-Intermediate-ffea00?style=flat-square)
![Java](https://img.shields.io/badge/Java-Intermediate-ffea00?style=flat-square)
![AI-MCP](https://img.shields.io/badge/MCP-Leaning-orange?style=flat-square)
![AI-Agents](https://img.shields.io/badge/Agents-Learning-orange?style=flat-square)

## Focus Areas

[![MCP](https://img.shields.io/badge/AI--Agent_Ready-MCP-green?style=flat-square)](https://modelcontextprotocol.io/)
[![Streamlit](https://img.shields.io/badge/UI-Streamlit-blue?style=flat-square)](https://streamlit.io/)
[![DuckDB](https://img.shields.io/badge/Database-DuckDB-blue?style=flat-square)](https://duckdb.org/)
[![Click](https://img.shields.io/badge/CLI-Click-blue?style=flat-square)](https://click.palletsprojects.com/)
[![Ansible](https://img.shields.io/badge/IaC-Ansible-blue?style=flat-square)](https://www.ansible.com/)
[![Terraform](https://img.shields.io/badge/IaC-Terraform-blue?style=flat-square)](https://www.terraform.io/)

---

## About Me
I’m a long-time Linux user (since the Slackware days) and active supporter of [Open Source Software][].
- Ubuntu user since 2005 (5.04), Ubuntu Member since ~2013
- Launchpad Package Maintainer since 2010
- Daily driver: Ubuntu & Oracle Linux (enterprise), Pop!\_OS for gaming, Alpine for containers

I’ve worked across Red Hat, Fedora, CentOS, Arch, Gentoo, and more. In short: if it’s Unix-y, I’ve probably used it.

---

## 🛰️ Current Focus: The Automated Radio Shack
I am bridging **Amateur Radio + AI workflows**, moving beyond static logging toward a modular, "Grand Central Station" architecture for station management.

- **Infrastructure as Code** → [Terraform][] & [Ansible][] with OCI, Nomad, Docker/LXC
- **Distributed Systems** → Vault, Consul, HA setups
- **Big Data & Propagation**
  - [wspr-ai-lite](https://github.com/KI7MT/wspr-ai-lite) — Lightweight DuckDB + Streamlit UI for multi-GB archive analysis.

---

## 🤖 Model Context Protocol (MCP) Hub
I am the architect of the **[ki7mt-mcp-hub](https://github.com/KI7MT/ki7mt-mcp-hub)** — a unified ecosystem of AI-agent micro-servers for Amateur Radio.

- **[adif-mcp](https://adif-mcp.com)** (`com.adif-mcp.validator`) — The authoritative validator for ADIF 3.1.6 log compliance.
- **[wspr-mcp](https://ki7mt.io/wspr)** (`io.ki7mt.wspr.researcher`) — Local AI access to gigabytes of propagation archives.
- **[qrz-mcp](https://ki7mt.io/qrz)** (`io.ki7mt.qrz.lookup`) — Specialized XML Callbook micro-service.
- **Station Control** → Roadmap includes `io.ki7mt.rig` for Hamlib integration and real-time SFI/K-index monitoring.

---

## 🛠️ The Tech Stack
- **Language/Env**: Python 3.12+, **[uv]** (for zero-config tool deployment)
- **Engines**: Ollama (Local LLMs), Qwen2.5-Coder (32B/7B)
- **Data**: DuckDB, ClickHouse, Apache Arrow, FastAPI/Uvicorn

This stack enables safe, contract-driven station automation, allowing AI agents to navigate logs and propagation data with high-fidelity precision.

---

## Home Lab
- EPYC 7302 128GB Linux AI Work Station
- Mac Studio 96GB AI Workstation
- 5950X TrueNAS Storage Server
- [Proxmox][] hypervisor for clustered VMs/containers
---

## Selected Projects
- [WSPR Analytics][] → Big Data exploration of WSPR spots
- [wspr-ai-lite](https://github.com/KI7MT/wspr-ai-lite) → portable DuckDB + Streamlit with MCP integration

---

## Let’s Connect
- Open for discussions on **Linux, DevOps, Amateur Radio, or AI Agents**
- Reach me on [GitHub Discussions](https://github.com/KI7MT/wspr-ai-lite/discussions)

---

<!-- Links (kept from your original for consistency) -->
[Open Source Software]: https://opensource.com/resources/what-open-source
[WSPR Analytics]: https://github.com/KI7MT/wspr-analytics
[WSPR]: https://www.physics.princeton.edu/pulsar/k1jt/wspr.html
[WSPRDAEMON]: http://wsprdaemon.org/
[Terraform]: https://www.terraform.io/
[Ansible]: https://www.ansible.com/
[Infastructure as Code]: https://developer.oracle.com/infrastructure-as-code/
[Nomad]: https://www.nomadproject.io/
[Proxmox]: https://www.proxmox.com/en/
[pfSense]: https://www.pfsense.org/
[US-XG-16]: https://store.ui.com/collections/unifi-network-switching/products/unifi-switch-16-xg
[USW-PRO-24 PoE]: https://store.ui.com/collections/unifi-network-switching/products/usw-pro-24-poe
[TrueNAS Core]: https://www.truenas.com/truenas-core/
[WSJTX UDP REST API]: https://github.com/KI7MT/wsjtx-logapi-go

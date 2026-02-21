Linux / DevOps Engineer | HF Propagation Prediction | Sovereign AI | Amateur Radio (KI7MT, DN13)

![Linux](https://img.shields.io/badge/Linux-Advanced-teal?style=flat-square)
![Bash](https://img.shields.io/badge/Bash-Advanced-teal?style=flat-square)
![Go](https://img.shields.io/badge/Go-Advanced-teal?style=flat-square)
![Python](https://img.shields.io/badge/Python-Advanced-teal?style=flat-square)
![C++/CUDA](https://img.shields.io/badge/C++/CUDA-Intermediate-ffea00?style=flat-square)
![ClickHouse](https://img.shields.io/badge/ClickHouse-Advanced-teal?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-Intermediate-ffea00?style=flat-square)

## Current Focus: IONIS-AI

**[IONIS-AI](https://github.com/IONIS-AI)** (Ionospheric Neural Inference System) — a self-hosted AI system that predicts HF radio propagation from the largest curated amateur radio dataset on Earth. 13+ billion spots. Zero cloud dependencies.

*The logs were speaking for decades, but nobody was listening. Now we're listening.*

[![IONIS](https://img.shields.io/badge/IONIS--AI-Propagation_Prediction-teal?style=flat-square)](https://github.com/IONIS-AI)
[![COPR](https://img.shields.io/badge/COPR-ionis--ai-blue?style=flat-square)](https://copr.fedorainfracloud.org/coprs/ki7mt/ionis-ai/)
[![ham-stats](https://img.shields.io/badge/Live-ham--stats.com-2ea043?style=flat-square)](https://ham-stats.com)

### The Stack

| Repo | Language | What It Does |
|:-----|:---------|:-------------|
| [ionis-apps](https://github.com/IONIS-AI/ionis-apps) | Go | High-performance data ingesters (22 Mrps) with watermark tracking |
| [ionis-core](https://github.com/IONIS-AI/ionis-core) | SQL/Shell | 34 ClickHouse DDL schemas, 13 population scripts |
| [ionis-cuda](https://github.com/IONIS-AI/ionis-cuda) | C++/CUDA | GPU-accelerated signature embedding engine |
| [ionis-training](https://github.com/IONIS-AI/ionis-training) | Python | PyTorch model training with physics-constrained sidecars |
| [ionis-docs](https://github.com/IONIS-AI/ionis-docs) | MkDocs | [Documentation site](https://ionis-ai.github.io/ionis-docs/) |

### The Data

| Source | Volume | What It Tells Us |
|:-------|:-------|:-----------------|
| WSPR | 10.8B spots (18 yrs) | SNR floor — path exists at minimum power |
| Reverse Beacon Network | 2.18B spots (17 yrs) | Skilled operator layer — CW through the noise |
| CQ Contest Logs | 195M QSOs | Ceiling — voice-workable at contest power |
| PSK Reporter | ~26M spots/day (live) | Operational — can a real operator make a contact? |
| DSCOVR L1 | Solar wind (live) | Predictive — Bz gives 15-45 min lead over Kp |

### The Model

**IONIS V20** (Production) — Pearson **+0.49** vs VOACAP +0.02. 84% recall on independent live data. 203K params, physics-constrained solar and geomagnetic sidecars. Every watt of inference runs on local hardware.

---

## About Me

Long-time Linux user (since the Slackware days) and active supporter of [Open Source Software][].

- Ubuntu user since 2005 (5.04), Ubuntu Member since ~2013
- RHEL/Fedora COPR packaging since ~2015
- Launchpad package maintainer since 2010
- Worked across Red Hat, Fedora, CentOS, Rocky, Arch, Gentoo, Alpine, and more

If it's Unix-y, I've probably broken it and fixed it.

---

## Sovereign AI Lab

Everything runs on local hardware. No cloud. No subscriptions. No vendor can revoke access.

| Host | Role | Specs |
|:-----|:-----|:------|
| **Threadripper 9975WX** | Control node | 32C/64T Zen 5, 128 GB DDR5, RTX PRO 6000 96 GB VRAM, Rocky Linux 9.7 |
| **Mac Studio M3 Ultra** | Training node | 96 GB unified memory, MPS backend for PyTorch |
| **EPYC 7302P** | Build/replica node | 16C/32T, 128 GB DDR4 ECC, Proxmox hypervisor |

**Networking**: 10 Gbps DAC point-to-point (Thunderbolt 4 + SFP+ AOC), MTU 9000
**Storage**: ClickHouse on dedicated NVMe (3.7 TB), ZFS archive pool (7.1 TB mirrored)
**Data platform**: ClickHouse (13B+ rows), PyTorch (MPS), Go ingesters (ch-go native protocol)

---

## MCP Servers

Architect of the **[ki7mt-mcp-hub](https://github.com/KI7MT/ki7mt-mcp-hub)** — AI-agent micro-servers for Amateur Radio.

- **[adif-mcp](https://adif-mcp.com)** — The authoritative validator for ADIF 3.1.6 log compliance
- **[wspr-mcp](https://ki7mt.io/wspr)** — Local AI access to propagation archives via DuckDB
- **[qrz-mcp](https://ki7mt.io/qrz)** — Specialized XML Callbook micro-service

---

## Let's Connect

Open for discussions on **Linux, DevOps, Amateur Radio, HF Propagation, or AI**.

Reach me on [GitHub Discussions](https://github.com/KI7MT/wspr-ai-lite/discussions) or via **ki7mt.io**

---

[Open Source Software]: https://opensource.com/resources/what-open-source

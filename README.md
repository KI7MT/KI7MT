Linux / DevOps Engineer | HF Propagation Prediction | Sovereign AI | Amateur Radio (KI7MT, DN13)

![Linux](https://img.shields.io/badge/Linux-Advanced-teal?style=flat-square)
![Bash](https://img.shields.io/badge/Bash-Advanced-teal?style=flat-square)
![Go](https://img.shields.io/badge/Go-Advanced-teal?style=flat-square)
![Python](https://img.shields.io/badge/Python-Advanced-teal?style=flat-square)
![C++/CUDA](https://img.shields.io/badge/C++/CUDA-Intermediate-ffea00?style=flat-square)
![ClickHouse](https://img.shields.io/badge/ClickHouse-Advanced-teal?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-Intermediate-ffea00?style=flat-square)

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
| **Threadripper 9975WX** | Control node | 32C/64T Zen 5, 128 GB DDR5, RTX PRO 6000 96 GB VRAM, Rocky Linux 9.8 |
| **Mac Studio M3 Ultra** | Training node | 96 GB unified memory, MPS backend for PyTorch |
| **EPYC 7302P** | Build/replica node | 16C/32T, 128 GB DDR4 ECC, Proxmox hypervisor |

**Networking**: 10 Gbps DAC point-to-point (Thunderbolt 4 + SFP+ AOC), MTU 9000
**Storage**: ClickHouse on dedicated NVMe (3.7 TB), ZFS archive pool (7.1 TB mirrored)
**Data platform**: ClickHouse (22B+ rows), PyTorch (MPS), Go ingesters (ch-go native protocol)

---

## Current Focus: QSO Graph

**[QSO Graph](https://github.com/qso-graph)** brings all of it together: research, AI/ML, propagation prediction and operating tools, for working the whole amateur radio ecosystem. A free desktop app for operators, MCP servers for the services hams use every day, and IONIS-AI propagation prediction.

[![qso-graph.io](https://img.shields.io/badge/qso--graph.io-Docs-teal?style=flat-square)](https://qso-graph.io)
[![Desktop](https://img.shields.io/github/v/release/qso-graph/qso-graph-desktop?label=QSO%20Graph%20Desktop&style=flat-square&color=2ea043)](https://github.com/qso-graph/qso-graph-desktop/releases/latest)
[![PyPI](https://img.shields.io/badge/PyPI-MCP_servers-blue?style=flat-square)](https://pypi.org/user/KI7MT/)

### QSO Graph Desktop

A free, open-source desktop app for amateur radio operators, for Windows, macOS and Linux: callsigns, locations, POTA, SOTA, ADIF, and a live WSJT-X Monitor.

- **macOS:** `brew install --cask qso-graph/tap/qso-graph-desktop`
- **Linux:** `apt install qso-graph-desktop` or `dnf install qso-graph-desktop`, from signed repositories at [packages.qso-graph.net](https://packages.qso-graph.net)
- **Windows:** signed installer from the [release page](https://github.com/qso-graph/qso-graph-desktop/releases/latest)

Every build is signed, macOS builds are notarized, and the app updates itself only when you say so. See the [install guide](https://github.com/qso-graph/qso-graph-desktop/blob/main/guide/install.md).

### MCP Servers

22 servers and 150 tools, each a separate package on [PyPI](https://pypi.org/user/KI7MT/), with credentials kept in the OS keyring and every outbound connection over HTTPS.

| Area | Servers |
|:-----|:--------|
| Logbooks and QSLs | [qrz-mcp](https://github.com/qso-graph/qrz-mcp), [lotw-mcp](https://github.com/qso-graph/lotw-mcp), [eqsl-mcp](https://github.com/qso-graph/eqsl-mcp), [hamqth-mcp](https://github.com/qso-graph/hamqth-mcp), [adif-mcp](https://github.com/qso-graph/adif-mcp) |
| On the air | [pota-mcp](https://github.com/qso-graph/pota-mcp), [sota-mcp](https://github.com/qso-graph/sota-mcp), [iota-mcp](https://github.com/qso-graph/iota-mcp), [netlogger-mcp](https://github.com/qso-graph/netlogger-mcp), [omiss-mcp](https://github.com/qso-graph/omiss-mcp), [n1mm-mcp](https://github.com/qso-graph/n1mm-mcp), [jt-mcp](https://github.com/qso-graph/jt-mcp), [dxe-mcp](https://github.com/qso-graph/dxe-mcp), [qso-graph-contest-mcp](https://github.com/qso-graph/qso-graph-contest-mcp) |
| Propagation and space weather | [solar-mcp](https://github.com/qso-graph/solar-mcp), [wspr-mcp](https://github.com/qso-graph/wspr-mcp), [ionis-mcp](https://github.com/qso-graph/ionis-mcp), [eme-mcp](https://github.com/qso-graph/eme-mcp), [meteor-mcp](https://github.com/qso-graph/meteor-mcp) |
| Zones and reference | [cq-zones-mcp](https://github.com/qso-graph/cq-zones-mcp), [itu-zones-mcp](https://github.com/qso-graph/itu-zones-mcp), [darc-dok-mcp](https://github.com/qso-graph/darc-dok-mcp) |

### IONIS-AI

**[IONIS-AI](https://github.com/IONIS-AI)** (Ionospheric Neural Inference System) — a self-hosted AI system that predicts HF radio propagation from one of the largest curated amateur radio datasets we are aware of. 22+ billion spots. Zero cloud dependencies.

*The logs were speaking for decades, but nobody was listening. Now we're listening.*

[![IONIS](https://img.shields.io/badge/IONIS--AI-Propagation_Prediction-teal?style=flat-square)](https://ionis-ai.com)
[![COPR](https://img.shields.io/badge/COPR-ionis--ai-blue?style=flat-square)](https://copr.fedorainfracloud.org/coprs/ki7mt/ionis-ai/)
[![ham-stats](https://img.shields.io/badge/Live-ham--stats.com-2ea043?style=flat-square)](https://ham-stats.com)

#### The Stack

| Repo | Language | What It Does |
|:-----|:---------|:-------------|
| [ionis-apps](https://github.com/IONIS-AI/ionis-apps) | Go | High-performance data ingesters (22 Mrps) with watermark tracking |
| [ionis-core](https://github.com/IONIS-AI/ionis-core) | SQL/Shell | 36 ClickHouse DDL schemas, 15 population scripts |
| [ionis-cuda](https://github.com/IONIS-AI/ionis-cuda) | C++/CUDA | GPU-accelerated signature embedding engine |
| [ionis-training](https://github.com/IONIS-AI/ionis-training) | Python | PyTorch model training with physics-constrained sidecars |
| [ionis-mcp](https://github.com/qso-graph/ionis-mcp) | Python | MCP server for propagation analytics (12 tools, [PyPI](https://pypi.org/project/ionis-mcp/)) |
| [ionis-jupyter](https://github.com/IONIS-AI/ionis-jupyter) | Python | Jupyter notebooks for propagation research (10 notebooks, [PyPI](https://pypi.org/project/ionis-jupyter/)) |
| [ionis-docs](https://github.com/IONIS-AI/ionis-docs) | MkDocs | [Documentation site](https://ionis-ai.github.io/ionis-docs/) |

#### The Data

| Source | Volume | What It Tells Us |
|:-------|:-------|:-----------------|
| WSPR | 12.9B spots (18 yrs) | SNR floor — path exists at minimum power |
| Reverse Beacon Network | 2.40B spots (17 yrs) | Skilled operator layer — CW through the noise |
| CQ Contest Logs | 388M QSOs | Ceiling — voice-workable at contest power |
| PSK Reporter | 7.2B spots (live) | Operational — can a real operator make a contact? |
| DSCOVR L1 | Solar wind (live) | Predictive — Bz gives 15-45 min lead over Kp |

#### The Model

**IONIS V22-gamma** (Production) — Pearson **+0.49** vs VOACAP +0.02. 98% recall on independent live data. 207K params, physics-constrained solar and geomagnetic sidecars. Every watt of inference runs on local hardware.

---

## Let's Connect

Open for discussions on **Linux, DevOps, Amateur Radio, HF Propagation, or AI**.

Reach me on [GitHub Discussions](https://github.com/KI7MT/wspr-ai-lite/discussions) or via **ki7mt.io**

---

[Open Source Software]: https://opensource.com/resources/what-open-source

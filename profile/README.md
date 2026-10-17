<div align="center">

<a href="https://openvcenter.com">
  <img src="https://raw.githubusercontent.com/openvcenter/Open-vCenter/main/.github/ovc-logo.svg" alt="Open vCenter" width="420" />
</a>

**An open-source virtualization center for managing your VMs from a single web console.**<br>
Microsoft Hyper-V today, more hypervisors through lightweight agents.

[Website](https://openvcenter.com) · [Live Demo](https://demo.openvcenter.com/) · [Documentation](https://openvcenter.com/docs/) · [Releases](https://github.com/openvcenter/Open-vCenter/releases) · [Issues](https://github.com/openvcenter/Open-vCenter/issues)

</div>

---

## 👋 About

Open vCenter (OVC) is a free, Apache 2.0 licensed web console for managing virtual infrastructure.
Browse your clusters, hosts and VMs, run lifecycle and power actions, edit hardware, manage
templates and ISOs, and open a VM console straight from the browser.

- 🖥️ **Centralized management** of clusters, hosts and virtual machines
- 🔓 **Fully open source**, with no paid tiers or locked features
- 🧩 **Agent-based architecture**, ready for new hypervisors
- 🤝 **Built in the open**: roadmap, issues and decisions are public

<p align="center">
  <img src="https://raw.githubusercontent.com/openvcenter/Open-vCenter/main/docs/screenshots/vm-details.png" alt="Open vCenter console" width="800" />
</p>

## 📦 Repositories

| Repository                                                                         | What it is                                                              |
| ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| **[Open-vCenter](https://github.com/openvcenter/Open-vCenter)**                    | Start here: overview, quick install (Docker Compose / Kubernetes), docs |
| **[Open-vCenter-Frontend](https://github.com/openvcenter/Open-vCenter-Frontend)**  | React web console                                                       |
| **[Open-vCenter-Backend](https://github.com/openvcenter/Open-vCenter-Backend)**    | FastAPI REST API + RabbitMQ worker (PostgreSQL, Valkey)                 |
| **[Open-vCenter-Agent-HyperV](https://github.com/openvcenter/Open-vCenter-Agent-HyperV)** | Go Windows service that runs on every Hyper-V host               |

```
Browser ──▶ Frontend ──REST──▶ Backend ──RabbitMQ──▶ Agent (one per host)
```

## 🚀 Getting started

```sh
git clone https://github.com/openvcenter/Open-vCenter.git
cd Open-vCenter/quick-install/docker
./up.sh
```

Open `http://localhost` and log in as `admin` / `admin`, then add your hosts from the console.
Full guides: **[Docker Compose](https://openvcenter.com/docs/docker-compose/)** · **[Kubernetes](https://openvcenter.com/docs/kubernetes/)** · **[Architecture](https://openvcenter.com/docs/architecture/)**

## 🗺️ Roadmap

| Area                                     | Status       |
| ---------------------------------------- | ------------ |
| Microsoft Hyper-V                        | ✅ Supported |
| vTPM and vGPU management                 | 🗓 Planned   |
| Host affinity / anti-affinity            | 🗓 Planned   |
| Automatic storage workload distribution  | 🗓 Planned   |
| Non-Hyper-V hosts (KVM / libvirt, ...)   | 🗓 Planned   |

## 🤝 Contributing

Contributions of all sizes are welcome: bug reports, docs and code.
Open an [issue](https://github.com/openvcenter/Open-vCenter/issues) in the main repository to report a bug or suggest a feature.

If Open vCenter is useful to you, consider giving the project a ⭐. It helps a lot!

---

<sub>Open vCenter is an independent open-source project and is not affiliated with, endorsed by, or sponsored by VMware, Broadcom, or Microsoft. All trademarks belong to their respective owners.</sub>

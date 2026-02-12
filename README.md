# Nexthink Dashboards

Pre-built dashboards for Nexthink Infinity — complete with JSON definitions you can import directly into your environment.

> **Part of [Butler DEX Enterprise](https://github.com/ButlerDEXEnterprise)** — At Your Enterprise's Service.

---

## 📋 Available Dashboards

| Dashboard | Category | Description | Tier |
|---|---|---|---|
| [DEX Score Overview](#dex-score-overview) | Executive | High-level view of your organization's digital experience health | 🟢 Free |
| [Device Health & Compliance](#device-health--compliance) | Operations | Uptime, disk space, OS versions, patch status at a glance | 🟢 Free |
| [User Experience / Login Times](#user-experience--login-times) | Performance | Login duration trends, slow logins by department, boot time breakdown | 🟢 Free |
| [Software License Optimization](#software-license-optimization) | Cost Savings | Unused licenses, underutilized software, reclamation candidates | 🔵 Premium |
| [VDI Performance](#vdi-performance) | Infrastructure | Latency, session quality, resource utilization across virtual desktops | 🔵 Premium |

<!-- Add rows as you publish more dashboards -->

---

## 🟢 Free Dashboards

### DEX Score Overview

**What it shows:** A single-pane executive view of your organization's digital experience — overall DEX score, trends over time, and breakdowns by department, location, or device type.

**Why it matters:** Leadership needs a simple answer to "how is our digital experience?" This dashboard gives them that answer without requiring them to understand NQL or dig through data.

**Use case:** Monthly executive reviews, DEX program tracking, before/after comparisons for improvement projects.

**Includes:** JSON definition + build guide explaining how each widget is constructed.

<details>
<summary>📥 Setup Instructions</summary>

1. Import the JSON definition into your Nexthink instance
2. Adjust filters for your organization (departments, locations, etc.)
3. Customize branding and thresholds as needed
4. Share with stakeholders

</details>

---

### Device Health & Compliance

**What it shows:** Fleet-wide view of device uptime, disk space, OS distribution, and patch compliance. Highlights devices that need attention with configurable thresholds.

**Why it matters:** This is the operational dashboard every IT team needs on day one. It surfaces the devices that are about to cause problems before they generate tickets.

**Estimated impact:** Proactive identification of at-risk devices reduces reactive support volume.

**Includes:** JSON definition + build guide.

<details>
<summary>📥 Setup Instructions</summary>

1. Import the JSON definition
2. Set your compliance thresholds (uptime, disk space, OS version)
3. Configure department or location breakdowns
4. Deploy to your operations team

</details>

---

### User Experience / Login Times

**What it shows:** Login duration trends across your environment — average, median, and 95th percentile. Breakdowns by department, device type, and location. Highlights users experiencing consistently slow logins.

**Why it matters:** Slow logins are the #1 user complaint in most enterprises, but IT rarely has visibility into the actual numbers. This dashboard makes the problem measurable and trackable.

**Use case:** Baseline before migrations, track improvement after GPO or profile changes, identify outlier devices.

**Includes:** JSON definition + build guide.

<details>
<summary>📥 Setup Instructions</summary>

1. Import the JSON definition
2. Adjust time range and grouping as needed
3. Set alert thresholds for slow logins
4. Share with desktop engineering and support teams

</details>

---

## 🔵 Premium Dashboards

### Software License Optimization

**What it shows:** Complete view of software usage across your fleet — identifies unused licenses, underutilized applications, and reclamation candidates with estimated cost savings per application.

**Why it matters:** Most enterprises overspend on software licenses by 20-40%. This dashboard makes the waste visible and quantifies the savings opportunity in dollars.

**Estimated savings:** Typically identifies 15-30% reclamation opportunity across major software titles.

> **This is a premium solution.** The dashboard approach and sample screenshots are documented here, but the production JSON and implementation guide are available through a consulting engagement. [Contact us](https://github.com/ButlerDEXEnterprise) to discuss your environment.

---

### VDI Performance

**What it shows:** Session quality, latency, resource utilization, and user satisfaction across your VDI environment. Correlates infrastructure metrics with actual user experience data.

**Why it matters:** VDI performance issues are notoriously hard to diagnose because the problem could be the endpoint, the network, the broker, or the host. This dashboard brings all the signals together in one view.

> **This is a premium solution.** [Contact us](https://github.com/ButlerDEXEnterprise) to discuss your environment.

---

## 🏗️ How Dashboards Are Built

Each dashboard folder includes:

| File | Description |
|---|---|
| `README.md` | What the dashboard shows, why it matters, and setup instructions |
| `dashboard.json` | The importable JSON definition — drop it straight into Nexthink |
| `BUILD_GUIDE.md` | Step-by-step explanation of how each widget was constructed in JSON |

The build guides are designed to teach you how to create your own dashboards — not just use ours.

---

## 📁 Repository Structure

```
nexthink-dashboards/
├── README.md
├── LICENSE
├── free/
│   ├── dex-score-overview/
│   │   ├── README.md
│   │   ├── dashboard.json
│   │   └── BUILD_GUIDE.md
│   ├── device-health-compliance/
│   │   ├── README.md
│   │   ├── dashboard.json
│   │   └── BUILD_GUIDE.md
│   └── user-experience-login-times/
│       ├── README.md
│       ├── dashboard.json
│       └── BUILD_GUIDE.md
└── premium/
    ├── software-license-optimization/
    │   └── README.md
    └── vdi-performance/
        └── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Nexthink Infinity with dashboard access
- Appropriate permissions to create and import dashboards
- Familiarity with Nexthink's dashboard JSON structure (or follow our build guides)

### Import a Dashboard
1. Review the README in the specific dashboard folder
2. Import the `dashboard.json` file into your Nexthink instance
3. Adjust filters, thresholds, and branding for your environment
4. Read the `BUILD_GUIDE.md` to understand how it was constructed
5. Customize and extend as needed

---

## ⚠️ Disclaimer

These dashboards are provided as-is. Always test in a non-production environment first. The author is not responsible for any unintended effects. This is not affiliated with or supported by Nexthink S.A.

---

## 📄 License

MIT License — free to use, modify, and contribute.

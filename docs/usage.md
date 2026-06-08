| [Home](../README.md) |
| -------------------- |

# Usage

The **System Overview** widget renders real-time system data on a FortiSOAR dashboard. It is the primary widget on the **System Health Status** dashboard — the first dashboard displayed when a user navigates to **Dashboard** — giving analysts and administrators an immediate view of platform and application health on login.

Each instance of the widget displays one monitoring view. Multiple instances can be placed on the same dashboard to present a comprehensive picture of system state side by side.

## What the Widget Displays

The content rendered by the widget depends on the **Choose Type of System Monitoring** value configured for that instance:

| Monitoring Type             | Displayed Information                                                                                                                      |
|-----------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| **Platform Health**         | Overall platform health percentage, CPU cores, memory (GB), storage (GB), and per-metric utilization percentages for CPU, memory, and disk |
| **Service Status**          | FortiSOAR internal services listed by category, each showing the count of active instances                                                 |
| **Connector Health Status** | All configured connectors listed by name, each showing current availability status                                                         |
| **Playbook Execution**      | Count of queued workflows, count of executed workflows, and percentage of disk space flagged for cleanup                                   |

## Interacting with the Widget

- **Refreshing** — click the refresh icon in the widget header to reload the displayed data with the latest values.
- **Collapsing** — click the collapse icon in the widget header to minimize the widget on the dashboard.
- For **Service Status** and **Connector Health Status**, click the expand arrow next to a service or connector name to view additional details.

## Example — System Health Status Dashboard

The **System Health Status** dashboard uses four instances of the **System Overview** widget to provide a complete operational snapshot of the FortiSOAR platform. The following configurations are used:

**Platform Health**

| Setting                              | Value           |
|--------------------------------------|-----------------|
| **Select Overview Type**             | Platform Health |
| **Choose Type of System Monitoring** | Platform Health |
| **Choose Data Size Type**            | Automatic       |
| **Color For CPU**                    | darkcyan        |
| **Color For Memory**                 | Cyan            |
| **Color For Disk**                   | lightcyan       |

Displays the overall platform health score alongside CPU, memory, and storage utilization metrics.

---

**Playbook Overview**

| Setting                              | Value                  |
|--------------------------------------|------------------------|
| **Select Overview Type**             | Application Monitoring |
| **Choose Type of System Monitoring** | Playbook Execution     |

Displays the count of queued workflows, total executed workflows, and the percentage of disk space available for cleanup.

---

**Service Status**

| Setting                              | Value           |
|--------------------------------------|-----------------|
| **Title**                            | Service Status  |
| **Select Overview Type**             | Platform Health |
| **Choose Type of System Monitoring** | Service Status  |

Lists all FortiSOAR internal services — such as AI, Application Workflow, Authentication & Access, and Web Gateway — each showing how many instances are active.

---

**Connector Health Status**

| Setting                              | Value                   |
|--------------------------------------|-------------------------|
| **Title**                            | Connector Health Status |
| **Select Overview Type**             | Application Monitoring  |
| **Choose Type of System Monitoring** | Connector Health Status |

Lists all configured connectors by name with their current availability status, allowing administrators to identify unavailable integrations at a glance.

## Next Steps

| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) |
| ---------------------------------------- | ------------------------------------------ |

| [Home](../README.md) |
| -------------------- |

# Installation

1. In FortiSOAR, navigate to **Content Hub** > **Discover**.
2. From the list of widgets, search for **System Overview**.
3. Click the **System Overview** widget card.
4. Click **Install** at the bottom of the card to begin installation.

# Configuration

To configure the **System Overview** widget:

1. Navigate to the dashboard where you want to add the widget.
2. Click **Edit Template** to open the template editor.
3. Click **Add Widget** and select **System Overview** from the list.
4. The **Edit System Overview** configuration form opens. Fill in the fields described in this section.
5. Click **Save** to apply the configuration.

You can add multiple instances of the **System Overview** widget to a single dashboard, each configured with a different monitoring type.

## Title

Enter a display name for the widget. This title appears in the widget header on the dashboard. If left blank, the widget renders without a header title.

## Select Overview Type

Select the broad monitoring category for this widget instance. The following overview types are available:

- **Platform Health** — displays metrics and status information about the FortiSOAR platform itself, such as resource utilization and service health.
- **Application Monitoring** — displays operational data about FortiSOAR applications and integrations, such as playbook activity and connector availability.

The option selected here determines which **Choose Type of System Monitoring** values are available, and which additional fields appear in the configuration form.

## Choose Type of System Monitoring

Select the specific monitoring view to display. The available options depend on the **Select Overview Type** selected:

| Overview Type          | Monitoring Type         | What It Displays                                                        |
|------------------------|-------------------------|-------------------------------------------------------------------------|
| Platform Health        | Platform Health         | Overall platform health score, CPU, memory, and storage metrics         |
| Platform Health        | Service Status          | Health status of FortiSOAR internal services, grouped by category       |
| Application Monitoring | Connector Health Status | Availability status of all configured connectors                        |
| Application Monitoring | Playbook Execution      | Counts of queued workflows, executed workflows, and disk cleanup status |

## Choose Data Size Type

Select the unit format used to display storage and memory values. This field appears only when **Select Overview Type** is set to **Platform Health** and **Choose Type of System Monitoring** is set to **Platform Health**.

The following options are available:

- **Automatic** — FortiSOAR selects the most appropriate unit based on the current value.
- Manual unit options may be available depending on your FortiSOAR version.

## Color For CPU / Color For Memory / Color For Disk

Select the display colors used for the CPU, memory, and disk metric values respectively. These color pickers appear only when **Select Overview Type** is set to **Platform Health** and **Choose Type of System Monitoring** is set to **Platform Health**.

Click the color swatch to open the color picker and choose a color. Each metric can be assigned an independent color to aid visual distinction at a glance.

## Next Steps

| [Usage](./usage.md) |
| ------------------- |

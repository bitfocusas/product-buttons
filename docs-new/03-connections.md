# Connections

**Connection** is where we link **Buttons** to the outside world: switchers, routers, software, hardware, and other imaginable (and unimaginable) options.

![Connection Window](../docs/3_connect/images/connection_1.png)

## Adding Connections

To start adding a connection, click the **+Add** button in the top-right corner of the left pane. This will display an extensive list of possible connections.

If no connections are visible, or you can't find the right module, you may need to update the library. Click *Download modules* in the top-right corner.

![Refresh Modules](../docs/3_connect/images/refresh.png)

This will bring up a popup box showing you the modules that are missing from your library or have newer versions.

![Upgrade Modules](../docs/3_connect/images/upgrade_modules.png)

Ensure you are online, as this process fetches the library from Bitfocus's servers. The download duration depends on your connection speed and the number of modules that will be downloaded.

Once the download is complete, you can search for the desired connection. Search by manufacturer, product line, or protocol. Generic connections can also be found by searching for the "generic" phrase.

![Create Connection](../docs/3_connect/images/create_1.png)

---

## Connection Badges

Each connection comes with a version dropdown and several informational badges.

### Router Badge

![Router Badge](../docs/3_connect/images/router_badge.png)

Indicates that the connection is supported by the Router system in Buttons. To filter the connections list for Router-supported options, click *Only Routers* at the top of the list.

### Legacy Badge

![Legacy Badge](../docs/3_connect/images/legacy_badge.png)

Indicates that the connection does not adhere to the latest API standards. While it may work, some features might be unavailable or non-functional.

### Pre-release Badge

![Pre-release Badge](../docs/3_connect/images/pre_release.png)

Indicates that the developer has released a test version of the module, and it may lack functionality or contain bugs.

---

## Version Management

![Version Number](../docs/3_connect/images/version_nr.png)

The **Version Dropdown** allows you to select between different versions of the connection as the library evolves.

![Available Versions](../docs/3_connect/images/available_versions.png)

You can also click the cogwheel to see and download other versions of the module.

---

## Configuring Connections

In the right pane of the connection page, you'll find all configuration options for the selected connection.

![Add Module](../docs/3_connect/images/add_module.png)

Some connections support MDNS to automatically discover devices, but it's good practice to know the connection settings beforehand. You can also enter the IP address for the connection manually. It's good practice to give each connection a clear and descriptive **Label** and **Variable Key**, so it's easy to recognize at a later stage.

![Add Module Details](../docs/3_connect/images/add_module_2.png)

### Swapping Module Versions

Under **Module** in the top right corner you can see the current module version in use for this connection. Clicking on it brings up a dialog box allowing you to swap the module versions.

![Swap Version](../docs/3_connect/images/swap_version.png)

---

## Connection Overview Tabs

### Actions Overview

![Action Overview](../docs/3_connect/images/action_overview.png)

View all available actions in the connection.

### Feedbacks Overview

![Feedback Overview](../docs/3_connect/images/feedback_overview.png)

View all available feedbacks.

### Variables Overview

![Variable Overview](../docs/3_connect/images/variable_overview.png)

View all variables exposed by the connection.

### Ports & Bundles Overview

![Ports and Bundles Overview](../docs/3_connect/images/ports_and_bundles_overview.png)

See what will be added to the Router system in Buttons.

---

## Module Information

![Module Info](../docs/3_connect/images/module_info.png)

These buttons allow you to:
- Navigate to GitHub to post a bug report
- Navigate to the repository
- Open the help file written by the module author

![Module Help](../docs/3_connect/images/module_help.png)

---

## View Options

![Connection View Options](../docs/3_connect/images/connection_view_options.png)

- **Log View**: Turn on debugging for the connection
- **Compact/Detailed View**: Toggle between views
- **Group/Sort**: Group and sort connections by tags

### Log View

![Log View](../docs/3_connect/images/log_view.png)

### Compact and Detailed Views

![Minimized View](../docs/3_connect/images/minimized_view.png) ![Maximized View](../docs/3_connect/images/maximized_view.png)

### Grouping Options

![Group View](../docs/3_connect/images/group_view.png)

---

## NMOS Connections

Under the **NMOS** section in the left pane of the connection page, you can find and set up NMOS devices available on your network.

![NMOS](../docs/3_connect/images/nmos.png)

If NMOS devices on your network announce themselves, they will appear and be available to connect to Buttons.

### Manual NMOS Creation

If devices are on another network segment or fail to appear, you can manually create the connection by clicking the **+Manual create** button. You'll need the IP address and port of the device.

![NMOS Manual](../docs/3_connect/images/nmos_manual.png)

Provide a name, IP address, and port number. For instance, a Blackmagic Design 2110 IP Video Converter 3x3G with IP `10.141.20.1` and port `8090`.

![NMOS Connected](../docs/3_connect/images/nmos_conected.png)

The NMOS connection is now ready for use in Buttons and will be available in the **Router Section** and on the **Routing Page**.


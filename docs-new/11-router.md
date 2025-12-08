# Router

The **Router Section** is an automated feature that populates itself with buttons similar to a standard XY router panel, based on router-compatible connections. This document covers both the Router Section in positions and the Routing UI pages.

---

## Router Section

### Creating a Router Section

1. Click on the starting cell

![Router Step 1](../docs/2_positions/images/router/router_1.png)

2. Click and drag to select cells. Minimum size: **6×2 cells**

![Router Step 2](../docs/2_positions/images/router/router_2.png)

3. Right-click and choose **Router**, or press **R**

![Router Step 3](../docs/2_positions/images/router/router_3.png)

The Router Section auto-populates with all Router-enabled connections, including Filter, Take, Delete, Auto, and Shuffle buttons.

![Router Created](../docs/2_positions/images/router/router_4.png)

---

## Router Layouts

![Router Inspector](../docs/2_positions/images/router/router_inspector2.png)

### Dual Layout (Default)

Two scrollable blocks for Sources and Destinations, with filter buttons in each block.

![Router Dual](../docs/2_positions/images/router/router_duo.png)

### Quad Layout

Filters occupy two blocks; Sources and Destinations share the remaining two. Ideal for frequent filter use with large workspaces.

![Router Quad](../docs/2_positions/images/router/router_quad.png)

### Mono Layout

Most button surface dedicated to either Destinations or Sources, with a toggle button to switch between them.

![Router Mono Sources](../docs/2_positions/images/router/router_mono.png)

![Router Mono Destinations](../docs/2_positions/images/router/router_mono2.png)

---

## Filtering

### Auto-Filter

The Router automatically filters Sources or Destinations as you interact with them.

![Router Auto Filter](../docs/2_positions/images/router/router_auto_filter.png)

Selecting **SDI1** on **NMOS A** as a Source filters Destinations to show only compatible NMOS destinations.

### Custom Filter Tags

![Router Filter](../docs/2_positions/images/router/router_filter.png)

Use filter buttons to refine results. Filter tags shown are system defaults; add custom tags in the **Tags** page.

### Limiting Sources and Destinations

Control which sources and destinations are available for your router panel using Tags.

#### Example: Producer Monitor

1. Create a tag (e.g., "Producer")

![Create Tag](../docs/2_positions/images/router/create_tag.png)

![Create Tag 2](../docs/2_positions/images/router/create_tag2.png)

2. Add the tag to relevant Destination bundles

![Add Destinations](../docs/2_positions/images/router/add_destinations.png)

3. Add the tag to relevant Source bundles

![Add Sources](../docs/2_positions/images/router/add_source2.png)

4. In the Router Inspector, set available sources and destinations to the **Producer** tag

![Change Router Tags](../docs/2_positions/images/router/router_tag_change_tags.png)

The router panel now shows only selected Sources and Destinations.

![Producer Router](../docs/2_positions/images/router/router_producer.png)

---

## Shuffle and Auto

Control which components of a source are routed to a destination. Note: Not all devices support component splitting.

### Auto Mode

![Router Auto 1](../docs/2_positions/images/router/router_auto_1.png)

Example of a two-part route:
- Video component from **SDI 1 Source**
- Audio and Data components from **SDI 4 Source** to **SDI 1 Destination**

![Router Auto 2](../docs/2_positions/images/router/router_auto_2.png)

### Shuffle View

For detailed component routing. Example: 64ch Madi destination and 4ch SDI input on an ATEM 4ME Constellation.

![Router Shuffle](../docs/2_positions/images/router/router_shufle.png)

Route any of the 4 source audio channels to any Madi destination. Press the purple **Destination** button to toggle between active sources and destinations.

---

## Router Inspector Options

![Router Inspector Full](../docs/2_positions/images/router/router_inspector_3.png)

### Scrollbar Position

![Scrollbar Position](../docs/2_positions/images/router/inspector/scrolbar_position.png)

Determine where navigation buttons appear. Remove them if your router section is on a surface with encoders.

### Layout Ratio

![Layout Ratio](../docs/2_positions/images/router/inspector/layout_ratio.png)

Move the dividing line between Sources and Destinations to accommodate different configurations.

### Options

![Options](../docs/2_positions/images/router/inspector/options.png)

- **Auto Take**: Automatically take a route when both destination and source are selected
- **Text Scroll**: Move oversized labels back and forth
- **Auto Close Filter**: Close filter dialogs after selection
- **Clear Selection After Take**: Clear selected sources/destinations after taking the route
- **Ignore Lock**: Override lock state on destinations

### Sorting Mode

![Sorting Mode](../docs/2_positions/images/router/inspector/sorting_mode.png)

- **Default**: Standard sorting
- **Labels Alphabetical (All)**: Alphabetical by label
- **Labels Alphabetical (Grouped)**: Grouped by connection, then alphabetical
- **Custom**: Based on custom sort column in the Labels page

![Custom Sort](../docs/2_positions/images/router/inspector/custom_sort.png)

![Custom Sort Surface](../docs/2_positions/images/router/inspector/custom_sort_surface.png)

### Ports

![Ports](../docs/2_positions/images/router/inspector/ports.png)

Configure **Auto Matching** options. Select which ports are available and matched. Turn off Audio and Data for video-only routing. Turn off "Show Auto Match Options" to remove the **Auto** button.

### Available Sources/Destinations

![Available Sources and Destinations](../docs/2_positions/images/router/inspector/available_sources_destinations.png)

By default, all Sources and Destinations appear. Use **Tags** to limit availability for specific Router Sections.

### User Filters

![User Filters](../docs/2_positions/images/router/inspector/user_filters.png)

By default, Buttons uses auto-generated filters. Add your own or remove auto-generated filters. Removing all filters removes the Filter buttons.

### Labels and Label Strategy

![Labels and Strategy](../docs/2_positions/images/router/inspector/labels_and_strategy.png)

Choose which label to use on Sources and Destinations:
- **Name**: Fetched from connections (always available)
- **Ext Custom Label**: User-definable label from connections (not always available)
- **User**, **Setup**, **Installation**: User labels created in the Labels section of Routing UI

![Label Strategy](../docs/2_positions/images/router/inspector/label_strategy.png)

**Label Strategy** defines fallback behavior. If no label exists in the chosen category, it falls back to the next option. Use "Off" only if all ports have labels in the chosen category.

### Styling

![Styling](../docs/2_positions/images/router/inspector/styling.png)

Change colors for Sources, Destinations, and Active Source. Set font size for buttons.

---

## Routing UI

The Routing UI consists of 4 pages.

### Config Page

![Routing Config](../docs/7_Routing/images/routing_config.png)

Read-only overview of all Ports and Bundles. Sort by clicking column headers. Filter by Sources/Destinations, Device, and Domain. Expand Bundles to see all ports.

### Labels Page

![Routing Labels](../docs/7_Routing/images/routing_label.png)

Assign customized labels to Ports and Bundles:
- **Name**: Fetched from connection
- **Ext Custom Label**: User-definable label from connection
- **User**, **Setup**, **Installation**: Custom labels

![Routing Labels 2](../docs/7_Routing/images/routing_labels-2.png)

Set custom sort values, icons, and colors for Bundles.

### Route Page

![Route Page](../docs/7_Routing/images/routing_route.png)

Route sources to destinations in dual-column style. Left column shows Destinations; right shows Sources.

Features:
- Route single bundles or single ports by expanding with **+**
- Expand all bundles with the **Ports** button
- Lock source/destination selection dropdowns together with the padlock button
- Swap selection between sources/destinations with the double arrow button

![Route 2](../docs/7_Routing/images/routing-route2.png)

Select multiple Sources and Destinations, then take the route directly or press **+** to add to a salvo.

![Route Salvo](../docs/7_Routing/images/route_salvo.png)

The Route Salvo popup allows you to:
- Remove single routes
- Clear the whole salvo
- Save the salvo
- Execute the salvo

### Salvo Page

![Salvo Page](../docs/7_Routing/images/routing_salvo1.png)

Create Salvos from scratch, edit existing salvos, and execute salvos.

> **Tip:** Internal Actions and Feedbacks exist for both Routes and Salvos, allowing single-button execution of complex routes and salvos.


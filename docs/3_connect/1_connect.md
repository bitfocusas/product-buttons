
**Connection** is where we link **Buttons** to the outside world: switchers, routers, software, hardware, and other imaginable (and unimaginable) options.  

![Connection window](images/connection_1.png)



To start adding **Connection**, click the **+Add** button in the top-right corner of the left pane. This will display an extensive list of possible connections.  

If no connections are visible, or you can't find the right module. You may need to update the library. To do this, click *Download modules* in the top-right corner. 
![Refresh](images/refresh.png)

This will bring up a popup box showing you the modules that are missing from your library or have newer versions.

![Upgrade modules ](images/upgrade_modules.png)

Ensure you are online, as this process fetches the library from Bitfocus's servers. The download duration depends on your connection speed and the number of modules that will be downloaded.

Once the download is complete, you can search for the desired connection. Search by Manufacturer, product line, or protocol. Generic connections can also be found by searching for the "generic" phrase.  
![Create](images/create_1.png)

### Connection Details

Each connection comes with a version dropdown and several informational badges.  

![Router Badge](images/router_badge.png)

**Router Badge**: Indicates that the connection supports the Router system in Buttons. To filter the connections list for Router-supported options, click *Only Routers* at the top of the list.  

![Legacy Badge](images/legacy_badge.png)

**Legacy Badge**: Indicates that the connection does not adhere to the latest API standards. While it may work, some features might be unavailable or non-functional.  

![Pre-Release](images/pre_release.png)

**Pre-release badge:** Indicates that the developer has released a test version of the module, and it may lack functionality or contain bugs.

![Version nr.](images/version_nr.png)

**Version Dropdown**: Allows you to select between different versions of the connection as the library evolves.

![Available versions](images/available_versions.png)

You can also click the cogwheel to see and download other versions of the module. 

### Adding a Blackmagic Design - ATEM Connection

To add the latest version of the *Blackmagic Design - ATEM* connection, click the **Add** button.



### Configuring Connections

In the right pane of the connection page, you’ll find all configuration options for the selected connection. 

![Add module](images/add_module.png)

Some connections support MDNS to automatically discover devices, but its good practice to know the connection settings beforehand. You can also enter the IP address for the connection manually. Its good practice to give each connection a clear and descriptive Label and Variable Key, so it's easy to recognize at a later stage.

![Add Module](images/add_module_2.png)

Under **Module** in the top right corner you can see the current module version in use for this connection, and by clicking on it you can bring up a dialog box allowing you to swap the module versions.

![Swap version](images/swap_version.png)

In addition to the Config View, you can also get an overview of the Actions available in the connection

![Action overview](images/action_overview.png)

There is also an overview of the available Feedbacks. 

![Feedback overview](images/feedback_overview.png)

And Variables.

![Variable overview](images/variable_overview.png)

Under Ports & Bundles you will get an overview over what will be added to the Router system in Buttons 

![Ports 6 Bundles overview](images/ports_and_bundles_overview.png)

![Module Info](images/module_info.png)

These buttons will allow you to navigate to Github to post a bug report or navigate to the repository. The help button will bring up the help file written by the module author.

![Module Help](images/module_help.png)

The Connection view option buttons 

![Connection View Options](images/connection_view_options.png)
  
- The first button will turn on the Log view, giving you opportunities to debug the connection.
- The second button will toggle between compact and detailed view
- The third button will allow you to group and sort the connections by tags

![Log view](images/log_view.png)

Logview.

![Minimized](images/minimized_view.png) ![maximized](images/maximized_view.png)

Minimized and Maximized view

![Group View](images/group_view.png)

Grouping options

We have now had a look at the different options for 1 module, there will be a lot of differences between the modules, but the main functionality will be the same. Take some time to familiarize yourself with the different options for the modules you will be using.


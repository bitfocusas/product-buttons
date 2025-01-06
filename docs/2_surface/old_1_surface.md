![Surface](images/surface.png)

When you click on the Surface button in the menu bar, it opens the window shown above. Initially, this window will display the surfaces available on the network you are connected to. It shows the type of surface, along with its IP address, port number, and serial number.

![Click on a surface](images/click_on_surface.png)

If you `click` on one of the surfaces, the context menu shown above will appear. For now, let’s `click` on **Adopt**.

![Surface Configuration](images/surface_configuration.png)

`Clicking` **Adopt** will add the surface to **Buttons**. `Click` it once more to open the Surface Config settings. Here, you can change the label of the surface, add tags, adjust the panel brightness, Reboot and use the Identify function, which flashes a button on the actual surface, making it easier to locate. You can also delete any surfaces that you don't want to control **Buttons**. Remember to `click`on **Save** when you are done. 


The ![Not assigned](images/not_assigned.png) informational by the surface indicates that the device is adopted in to **Buttons** but is currently not in use on any **Positions**

![Not assigned context](images/not_assigned_context.png)

If you`click`on that informational it will bring up a context menu where you can either **Create Position** or depending on your current configuration assign it to an existing **Position** In this setup we have already set up a few positions.

You can also `click`on the blue ![+add](images/+add.png) button to manually set up a surface.

![Create a surface select model](images/create_surface1.png)

This will bring up the create surface selection dialog box. Let's select an iPad.

![Create a surface select model](images/create_surface2.png)

And then give it a name and `click` **Create surface.**

![Create a surface select model](images/ipad_surfaceconfig.png)

This will bring up the Surface config page for the iPad Surface we just crated
If you want to have a look at it just click on the green ![Create a surface select model](images/open_ipad_view.png) button, this will bring up a ipad view in the browser that you can use as a surface 

![Create a surface select model](images/ipadview2.png)

If you want to bring this view to an actual iPad you will have to exchange the loop back IP address 127.0.0.1 with the actual ip address of the machine running **Buttons** in this case 192.168.0.252 so the full URL in this case would be:
`http://192.168.0.252:3000/ipad/3699635a-77fa-4770-8263-071eca7758f3`but this will of course be different in your case both the IP adress and the ID of the **Surface** which is the last part of the URL

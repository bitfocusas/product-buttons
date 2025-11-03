![Position](images/position/positions.png 'Position')

**Position** defines a collection of one or more **Surfaces**. It typically aligns with the working role of an individual, such as Vision Mixer, Graphics, or Shader. Each **Position** can be tagged for better **Organization**. To create a new **Position**, click the **+Create** button at the top of the left pane. 

A dialog box will appear, prompting you to enter a label for the **Position**. It's a good idea to plan your naming conventions beforehand to maintain a logical and consistent system. You can also create **Positions** when configuring your **Surfaces**.

![Create position](images/position/create_position.png 'Create Position')

**Click** *Create Position*, and the **Position Editor** window will open.

![Position editor window](images/position/position_editor_window.png 'Position Editor Window')

The **Position Editor** window consists of three panes:
- **Left Pane**: Navigation tree  
- **Middle Pane**: A 16x16 grid called the **Canvas**  
- **Right Pane**: Contains **Inspector**, **Presets**, and **Configuration** tabs  

To gain more space for editing in the position view, you can minimize the left pane.

![minimize](images/position/minimize_button.png)

**Configuration view**

![Configuration](images/position/configuration_1.png 'Configuration')

Here, you can change the name, add a description for the **Position**, and assign **Surfaces** to it.

![Configuration_2](images/position/configuration_2.png 'Configuration_2')

**Click** *Assign Surface* and select the desired **Surface**.

![Configuration 3](images/position/configuration_3.png 'Configuration 3')

The selected **Surface** will appear in the **Canvas** in the **Configuration** tab. A corresponding outline will also display in the center pane **Canvas**, showing the part of the **Canvas** covered by the **Surface**. You can move the **Surface** to your preferred position on the **Canvas** by dragging it in the **configuration window**. let's add another **Surface**.

![Configuration 4](images/position/configuration_4.png 'Configuration 4')

Now, there are two **Surfaces** assigned to the **Position**. The outlines correspond to the button layouts of the assigned **Surfaces**:  
- The **STREAM DECK STUDIO** has two rows of 16 buttons.  
- The **STREAM DECK XL** has four rows of 8 buttons.  

You can combine **Surfaces** freely within the same **Canvas**. You can move surfaces around from the **Configuration** window, by clicking on a surface and draging it to a new position. Overlapping parts of **Surfaces** will display shared buttons on both.

![move](images/position/move_surface.png)

---

With Position variable, you can assign variables to your positions.

The definition of the variables are shared between all positions, while each position has its own current and initial value, independently of each other.  
The values can also be used by any shared section used in a position, and will get the value from the position they are mounted on.


![Position Variable](images/position/position_variable_2.png)

![Position Variable](images/position/position_variable_3.png)


![Click inside any rectangle](images/position/click_inside_any_rectangle.png 'Click inside any rectangle')  

**Click** inside any rectangle on the **Canvas**; its outline will become dashed, indicating it's selected. **Right-click** to open the context menu. From here, you can create a **Button**, **Section**, **Shift Section**, **Folder Section**, **Popover**, **Router** or **Shared Section**. The **Paste** and **Clear Selection** options are self-explanatory, but the other features will be explained further.

![Right Click](images/position/right_click.png 'Right Click')

**Click** on **Button**. or you could simply press **B** instead of right clicking and selecting from the context menu.

![Click on Button](images/position/button_on_grid.png 'Click on Button')

You have now created a **Button**.

![Side pane](images/position/side-pane_callout.png 'Side Pane')

To optimize your workspace, you can move the **Inspector** pane from the side pane to the bottom of the screen. This setting provides more real estate for making multiple edits without excessive navigation.

![Bottom Pane](images/position/bottom-pane_callout.png 'Bottom Pane')
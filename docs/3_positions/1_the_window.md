# Position
![position](images/positions.png 'position')
Position is how we define a collection of one or multiple surfaces, It also typically aligns with the working position of a person for example Vision Mixer, Graphics or Shader. Each position may be Tag'ed for better Organization. You can create a new position by pressing the (+create) in the top of the left pane
You will then be presented with a dialog box to enter a label for the position. Some planing regarding naming conventions is smart so that the system will be logical and consistent.
![Create position](images/create_position.png 'create poition')
Click Create position, and the position editor window will open.
![Position editor window](images/position_editor_window.png 'position editor window')
The position editor window has 3 panes the left which is the Navigation tree, the middle which is a 16x16 button grid and the right which contains Inspector, Presets and Configuration.
![Inspector](images/inspector.png 'inspector')
The inspector will show the grid size of 16W and 16H let's leave it at that for now, but it can be changed at any time.
![Click'n drag](images/click_and_drag.png 'click`n drag')
Click´n drag a section of 16x2 buttons in the button grid and right click inside the selection. Just ignore the yellow box in the lower right corner for now we will get back to that.
![Right click](images/right_click.png 'right click')
you will now be presented with a few choices **Button**, **Section**, **Shift Section**, **Popover** and **Plugins**.

**Paste** and **Clear selection** is kind of self-explanatory, but we will go through the others

**Buttons** and **Plugins** are "action" handlers they do the work while the different **Sections** are more organizational. 

**Button** will create 32 buttons in a 16x2 grid quick and easy. We will get back to how you configure the buttons. **Buttons** are the basic "action" handler we will 

**Plugin** Will create a premade "application" for example the Crosspoint routing application, which will make setting up Crosspoint routing a breeze. We will get back to both the Crosspoint and more about plugins later.

**Section** will create a parent "container" which can hold children *Buttons*, *Sections*, *Shift Sections*, *Popovers** and *Plugins* or any combination thereof for organizational purposes.

**Shift Section** will create a parent "container" which can hold children *Buttons*, *Sections*, *Shift sections*, *Popovers* and *Plugins* and have one or multiple page button that will give you access to subpages for the section, expanding the available grid space.

**Popover** will create a parent "container" which can hold children *Buttons*, *Sections*, *Shift sections*, *Popovers*, and *Plugins* and will unfold end expand over the underlying objects on the grid.


We have used the terms Parent and Children quite a lot in the preceding paragraph and if you take a look at the Tree in the left pane in the picture below the relationship between Parent and children should be self-evident
![populated](images/populated.png 'populated')
You can re-arrange, move and rename *Buttons* and *Sections* both in the tree and in the grid
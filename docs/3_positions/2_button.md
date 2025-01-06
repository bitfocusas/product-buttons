![Button](images/button/button.png 'Button')

A **Button** is a fundamental action handler. You push it, and something happens. It has many properties, which we will explore step by step.

The first thing to notice is the *8 dots* in the top-left corner of a selected **Button**. This is the *Handle Bar*. When you hover over it, your mouse will change to an open hand, allowing you to click and drag the button around the **Canvas**.

![Button properties 1](images/button/button_properties_1.png 'Button properties 1')

### **Button Properties Overview**
- **Label**: The name of the **Button** displayed in the tree view.
- **Style**: Determines the layout of the **Button**:
  - Icon and one line of text (Default).
  - Icon only.
  - Three lines of text where the top line has distinct color properties.
  - Three lines of text where the middle line is larger than the others.

- **Icon**: Select an icon from a dropdown or use the search bar.  
  You can also click the `x` to upload a **PNG** file as an icon.

![Icon](images/button/icon.png 'Icon')  
![Upload png1](images/button/upload_png1.png 'Icon')  
![Upload png 2](images/button/upload_png_2.png 'Icon')

### **Text Fields**
Text fields depend on the chosen button style:  
![Button properties 2](images/button/button_properties_2.png 'Button properties 2')
- **Context**: The top line in the third and fourth styles.
- **Text**: The middle line in the third and fourth styles (or the only line in the first style).
- **Text 2**: The bottom line in the third and fourth styles.

Each text box includes a **Variable Selector** button, which opens a dialog for browsing and selecting available system variables.

![Variable Selector Dialog](images/button/var_sel_dialog.png 'Variable Selector Dialog')  
![Button properties 3](images/button/button_properties_3.png 'Button properties 3')  
![Button variable](images/button/button_variable.png 'Button variable')

### **Styling**
![Button Properties 4](images/button/button_properties_4.png 'Button Properties 4')  
![Button styling](images/button/button_styling.png 'Button styling')

### **Location**
![Location](images/button/location.png 'Location')

- **Flow** determines button behavior and positioning:
  - **Float**: Positions dynamically, starting from top-left.
  - **Static**: Allows full customization by setting X/Y coordinates (Default).
  - **Anchor**: Automatically positions the button in corners, allowing resizing.
  - **Fixed**: Similar to anchor but unaffected by scrolling.

### **Action Handling**
![Action 1](images/button/action_1.png 'Action 1')

Actions connect the **Button** to **Connections** or internal functions. Action handlers include:
- **Press**: Executes when the button is pressed.
- **Release**: Executes when released.
- **Left/Right**: Assigns actions an action to the left rotation and another to the right rotation **SDS**.
- **Encoder**: Assigns both left and right rotations to a single Action and the Delta is used to adjust the value of the action **SDS**.

For example, we’ll use the *Press Action Handler*:  
![Add Action](images/button/action_add_action.png 'Add Action')

1. **Click** on *+ Add Action* and select an action.  
2. Use the search and filter menu for large **Connections** lists.  

![Action Search](images/button/action_search.png 'Action Search')  
![Action Search 2](images/button/action_search_2.png 'Action Search 2')

**Example:** Select *ME:Set Program Input*. The button will set the Atem switcher’s Program bus to input 1.  

![Action 3](images/button/action_3.png 'Action 3')  
Update the button text with variables for dynamic display:  
![Button Variable Atem](images/button/button_variable_atem.png 'Button Variable Atem')  
![Button with Variable](images/button/button_with_variable.png 'Button with Variable')

### **Action Steps**
Buttons can act as playlists, performing multiple actions sequentially:  
![Action Dialog](images/button/action_1.png 'Action Dialog')  
- Add steps by clicking the *+* after *Step 1*.  
- Each step has unique **Style** and **Action** dialogs.  
- Under the `cogwheel` you find an option to set auto-progress through steps with delays.

![Action 4](images/button/action_4.png 'Action 4')  

Delays can be set to **Absolute** or **Relative**:  
- **Absolute**: Actions start a set time after button press (Default).  
  ![Absolute Delay](images/button/delay-absolute.jpg 'Absolute Delay')  
- **Relative**: Each action runs a set time after the previous one starts.  
  ![Relative Delay](images/button/delay-relative.jpg 'Relative Delay')  

### **Feedback**
The **Feedback** tab adjusts button appearance based on conditions.  

![Feedback Dialog](images/button/feedback.png 'Feedback Dialog')  
- **Click** on *+ Add Feedback* and configure conditions.  
- Example: Adjust button text or style when input 1 is live.  

![Feedback Example](images/button/feedback_3.png 'Feedback Example')

### **Testing Buttons**
Test buttons without a surface by holding **Shift** and clicking.  

![Execute Mode](images/button/execute_mode.png 'Execute Mode')  
You can also execute actions directly within the action dialog:  
![Execute in Action](images/button/execute_in_action.png 'Execute in Action')

---

This concludes the **Button** overview. Up next: **Presets**, a faster method for configuring buttons.
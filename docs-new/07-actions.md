# Actions and Feedbacks

Actions connect buttons to connections or internal functions. This document covers action handlers, action steps, action groups, action logic, feedbacks, and repeaters.

---

## Action Handlers

![Action Handlers](../docs/2_positions/images/button/action_1.png)

Action handlers determine when actions execute:

- **Press**: Executes when the button is pressed
- **Release**: Executes when the button is released
- **Left**: Assigns an action to left rotation (Stream Deck Studio/Plus)
- **Right**: Assigns an action to right rotation (Stream Deck Studio/Plus)
- **Encoder**: Assigns both left and right rotations to a single action using delta values (Stream Deck Studio/Plus)

---

## Adding Actions

![Add Action](../docs/2_positions/images/button/action_add_action.png)

You can search directly in the **+ Add Action** field, or click on the folder icon at the end to bring up the Action selection dialog box.

![Action Search](../docs/2_positions/images/button/action_search.png)

### Example: ATEM Switcher

Select *ME:Set Program Input*. The button will set the ATEM switcher's M/E 1 bus to the specified input.

![Action Configured](../docs/2_positions/images/button/action_3.png)

---

## Action Steps

Buttons can act as playlists, performing multiple actions sequentially.

![Action Steps](../docs/2_positions/images/button/action_4.png)

### Managing Steps

- Add steps by clicking the **+** after *Step 1*
- Use the duplicate step button to copy an existing step
- Each step has unique **Style** and **Action** dialogs
- Under the **cogwheel**, find options for auto-progress (each press advances to the next step)
- Choose between absolute or relative delays

### Renaming Steps

Double-click on a step to bring up a dialog box where you can change the name.

![Rename Step](../docs/2_positions/images/button/rename_step.png)

### Reordering Steps

Use the reorder option to drag steps into the position you need.

![Reorder Steps](../docs/2_positions/images/button/reorder_steps.png)

---

## Delays

### Absolute Delays

Actions start a set time after the button press (Default).

![Absolute Delay](../docs/2_positions/images/button/delay-absolute.jpg)

### Relative Delays

Each action runs a set time after the previous one starts.

![Relative Delay](../docs/2_positions/images/button/delay-relative.jpg)

---

## Action Groups

When clicking on **+Add Action**, you are presented with options to create an **ActionGroup** or **ActionLogic**.

![Recently Used Actions](../docs/2_positions/images/button/action_recently_used.png)

### ActionGroup

ActionGroup lets you group different actions together for either:

- **Sequential**: Actions run one after another
- **Concurrent**: Actions run simultaneously

![Action Group](../docs/2_positions/images/button/action_group.png)

---

## Action Logic

ActionLogic lets you create conditional actions that only execute if certain conditions are met.

For conditions, you can use any feedback or use an expression to test a variable for a value.

### Example: Time-based Condition

In this example, we test the `$(time.hh)` variable for a value larger than or equal to 12 on a 24-hour clock. This determines whether it's after noon (true) or before noon (false).

![Condition Setup](../docs/2_positions/images/button/action_logic_condition.png)

### When True

If the time is between 12:00 and 23:59, pressing the button will set the light to 255 (100%).

![When True Action](../docs/2_positions/images/button/action_logic_true.png)

### Else

If the time is between 00:00 and 11:59, pressing the button will set the light to 128 (approximately 50%).

![Else Action](../docs/2_positions/images/button/action_logic_else.png)

### Stacking Action Logic

You can stack multiple ActionLogics testing for different conditions, resulting in multiple different actions being executed if conditions are true.

![Action Logic Group](../docs/2_positions/images/button/action_logic_group.png)

---

## Feedbacks

The **Feedback** tab adjusts button appearance based on conditions.

![Feedback Tab](../docs/2_positions/images/button/feedback.png)

As with Actions, you can search directly in the **+ Add Feedback** field, or click on the folder icon to bring up the Browse feedback dialog box.

![Feedback Dialog](../docs/2_positions/images/button/feedback_dialog.png)

### Multiple Feedbacks

There is an option in the dialog box to select multiple feedbacks. For example, you can select both **ME:One ME preview source** and **ME:One ME Program source**.

![Feedback Example](../docs/2_positions/images/button/feedback_3.png)

This brings two feedbacks into the button properties. Change the color for the **ME:One ME preview** feedback to green and leave the **ME:One ME Program** feedback as is.

- Button turns **red** when Camera 1 is live on the Program bus
- Button turns **green** when Camera 1 is in the Preview bus

![Live on Program](../docs/2_positions/images/button/button_red.png) ![Live on Preview](../docs/2_positions/images/button/button_green.png)

---

## Repeaters

In some connections, settings are made into dropdown lists, enabling the repeater function.

![Dropdown](../docs/2_positions/images/button/action_dropdown.png)

### Creating Action Repeaters

Click on the **...** menu inside the dropdown box to bring up the repeater options.

![Repeater Menu](../docs/2_positions/images/button/action_repeater2.png)

Click on **Create repeater** to automatically create a button for each item in the dropdown list.

![Controlled by Repeater](../docs/2_positions/images/button/controled_by_repeater.png)

This creates 18 buttons from one single button. The first button becomes a master—if you change any styling on that button, it changes on all the "children."

![Repeater Buttons](../docs/2_positions/images/button/repeater_buttons.png)

### Feedback Repeaters

Enable the repeater function on feedbacks as well.

![Repeater Feedback](../docs/2_positions/images/button/repeater_feedback.png)

Now you have 18 buttons with feedback for both Program and Preview.

![Repeater Buttons with Feedback](../docs/2_positions/images/button/repeater_buttons_2.png)

### Customizing Repeated Buttons

At the bottom of the Inspector, you'll find repeater options.

![Repeater Options](../docs/2_positions/images/button/repeater_options.png)

Click on **Customize** to bring up a dialog box.

![Customize Label](../docs/2_positions/images/button/customize_1.png)

In the generated buttons window, you can customize labels, icons, and colors depending on the button style chosen for the master button.

![Customize with Icon Style](../docs/2_positions/images/button/customize_3.png)

### Hiding Sources

In the "All Available Data" window, you can hide buttons for sources you don't need.

![Customize Sources](../docs/2_positions/images/button/customize_2.png)

Click on the "eye" icons to hide/unhide sources.

![Customize Sources 2](../docs/2_positions/images/button/customize_4.png)

### Result

With a few clicks, you can create a simple controller for an ATEM 1ME mixer with selected sources and both Program and Preview feedbacks.

![Customized Buttons](../docs/2_positions/images/button/customized_buttons.png)


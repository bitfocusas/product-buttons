# Sections

The canvas can be divided into different sections that can be resized and moved as needed. This document covers all section types: basic sections, shift sections, folder sections, popovers, and shared sections.

---

## Basic Sections

### Creating a Section

![Create Section Step 1](../docs/2_positions/images/section/create_section_1.png)

1. **Start a Section**: Click on the cell where you want to begin. A bounding box appears around the selected cell.

![Create Section Step 2](../docs/2_positions/images/section/create_section_2.png)

2. **Expand the Section**: Click and drag to include the desired cells. When you release, the bounding box expands to encompass all selected cells.

![Create Section Step 3](../docs/2_positions/images/section/create_section_3.png)

3. **Create the Section**: Right-click to open the context menu and select **Create Section**, or press **S**.

![Create Section Step 4](../docs/2_positions/images/section/create_section_4.png)

The section includes handles for adjusting size and shape. A **section marker box** appears in the top-left corner. Use the handlebar within the section bar to move the entire section across the canvas.

---

## Section Inspector

![Section Inspector](../docs/2_positions/images/section/section_inspector.png)

- **Style**: Set main and secondary colors to distinguish sections
- **Location**: Adjust position and size
- **Pages/Scroll**: Define behavior when the section becomes "overfilled"
- **Variables**: Create section-specific variables
- **Authentication**: Set PIN code or NFC security

---

## Scrolling and Pages

### Handling Overflow

![64 Button Section](../docs/2_positions/images/section/section_64btn.png)

With 64 buttons in a section, changing the size to 8×2 shows this:

![64 Buttons Overflow](../docs/2_positions/images/section/section_64btn_2.png)

A warning about **Item Overflow** appears with an option to **Enable Scroll**.

![Enable Scroll](../docs/2_positions/images/section/section_64btn_3.png)

When scroll is enabled, navigation buttons appear. If using a **Stream Deck Studio**, you can also use encoders to scroll through buttons.

### Pages/Scroll Settings

![Pages/Scroll Settings](../docs/2_positions/images/section/pages_scroll.png)

Configure:
- Position and visibility of navigation buttons
- Push encoder to switch control between sections (connected section flashes, encoder color matches section's main color)

This feature is convenient for expanding button capacity—for example, accessing 100+ PTZ camera presets efficiently without displaying all at once.

---

## Authentication

![Authentication](../docs/2_positions/images/section/authentication.png)

Protect buttons from accidental activation or unauthorized access using PIN codes or NFC key fobs (Stream Deck Studio).

### PIN Code Rules

![Code Rule](../docs/2_positions/images/section/code_rule.png)

Add multiple code rules as needed. Codes must be numerical. Set auto-lock time after unlocking.

![Locked Section](../docs/2_positions/images/section/locked%20_section1.png)

Pressing a button within a locked section brings up the code panel:

![Code Panel](../docs/2_positions/images/section/codepanel.png)

### NFC Rules

![NFC Rule](../docs/2_positions/images/section/nfc_rule.png)

Select **Add NFC Rule**. Hold an NFC key fob, sticker, or compatible device near the Stream Deck Studio reader. It will be detected and added as a locking/unlocking method.

![Code + NFC Locked](../docs/2_positions/images/section/code_nfc_locked.png)

When both rules are active, unlock by entering the code or holding the NFC device near the reader.

> **Tip:** Use the NFC reader on the Stream Deck Studio to authenticate any section on any Stream Deck in the Position.

---

## Shift Sections

The **Shift Section** effectively doubles available space by adding an additional layer of cells, accessible with a single button press.

### Creating a Shift Section

1. Click on the starting cell

![Shift Section Step 1](../docs/2_positions/images/shift_section/shift_section_1.png)

2. Click and drag to select desired cells

![Shift Section Step 2](../docs/2_positions/images/shift_section/shift_section_2.png)

3. Click **Shift Section** or press **Shift+S**

![Shift Section Step 3](../docs/2_positions/images/shift_section/shift_section_3.png)

![Shift Section Created](../docs/2_positions/images/shift_section/shift_section_4.png)

> **Tip:** Turn off the **Shift** button and use the internal action *Set Active Page* to navigate between Main and Shift pages with custom navigation.

### Use Cases

Shift Sections are useful for setups like PTZ camera presets:

- **Main Layer**: Recall functions
- **Shift Layer**: Save functions

![Shift Recall](../docs/2_positions/images/shift_section/shift_section_recall.png)

![Shift Save](../docs/2_positions/images/shift_section/shift_section_save.png)

Making the section scrollable fits even more buttons within the same cells.

---

## Folder Sections

**Folder Sections** function similarly to Shift Sections but with multiple layers. Navigate using folders and subfolders.

### Creating a Folder Section

1. Click on the starting cell

![Folder Section Step 1](../docs/2_positions/images/folder_section/folder_section_1.png)

2. Click and drag to select cells

![Folder Section Step 2](../docs/2_positions/images/folder_section/folder_section_2.png)

3. Right-click and choose **Folder Section**, or press **F**

![Folder Section Step 3](../docs/2_positions/images/folder_section/folder_section_3.png)

The section is created with 3 folders as a default.

![Folder Section Created](../docs/2_positions/images/folder_section/folder_section_4.png)

### Managing Folders

![Folder Section Inspector](../docs/2_positions/images/folder_section/folder_section_5.png)

In the Inspector's **Navigation** dialog:

- View **Main** and subfolders
- Add subfolders with **+ Add Folder**
- Drag folders onto other folders to create subfolder hierarchy
- Rename folders
- Change colors and icons
- Modify folder layout order (left-to-right or top-to-bottom)
- Adjust the return button within each folder
- Turn off folder navigation buttons
- Turn off the return button

> **Tip:** Use the internal action *Set Active Page* to create custom navigation.

---

## Popovers

**Popover Sections** expand from a single button—ideal for functions you want accessible but don't use frequently.

### Creating a Popover

1. Click on the starting cell

![Popover Step 1](../docs/2_positions/images/popover/popover_1.png)

2. Click and drag to select cells for the unfolded size

![Popover Step 2](../docs/2_positions/images/popover/popover_2.png)

3. Right-click and choose **Popover**

![Popover Step 3](../docs/2_positions/images/popover/popover_3.png)

Even though you selected multiple cells, only the starting cell is initially occupied.

![Popover Created](../docs/2_positions/images/popover/popover_4.png)

4. Click the **Open/Close** button at the end of the section bar to view and edit

![Popover Open](../docs/2_positions/images/popover/popover_5.png)

### Popover Inspector

![Popover Inspector](../docs/2_positions/images/popover/popover_inspector.png)

Customize:

- **Color and Icon**: Appearance of the Popover button
- **Section Color**: Color of the expanded section
- **Size and Direction**: Section size and unfolding direction
- **Position Offset**: Offset the section away from the button
- **Animation**: Toggle open/close animation
- **Dismiss on Click**: Automatically close after pressing a button inside

---

## Shared Sections

**Shared Sections** can be embedded in multiple positions, sharing a common set of buttons. Changes to a shared section update everywhere it's used.

### Creating a Shared Section

![Shared Section Location](../docs/2_positions/images/shared_section/shared_section_1.png)

Find **Shared Section** under the position in the navigation tree.

![Shared Section Menu](../docs/2_positions/images/shared_section/shared_section_2.png)

Click **+Create** and enter a name and size.

![Shared Section Dialog](../docs/2_positions/images/shared_section/shared_section_3.png)

You get a canvas with the specified size.

![Presets in Shared Section](../docs/2_positions/images/shared_section/presets_2.png)

Add buttons manually or from presets.

### Embedding a Shared Section

![Create Shared Section](../docs/2_positions/images/shared_section/create_shared_section.png)

Go into a position, select cells matching your shared section size, right-click, and select **Shared Section**.

![Choose Section](../docs/2_positions/images/shared_section/choose_the_section.png)

Choose from available shared sections.

![One Shared Section](../docs/2_positions/images/shared_section/one_shared_section.png)

The shared section appears with all its buttons.

![Multiple Shared Sections](../docs/2_positions/images/shared_section/6_shared_section.png)

Reuse it as many times as needed across one or multiple positions.

### Editing Shared Sections

![Back Navigation](../docs/2_positions/images/shared_section/back_navigation.png)

Click on the shared section to bring up the section bar with a button to navigate directly to the shared section for editing.

> **Tip:** When placed in a Position, shared sections have access to that Position's variables.


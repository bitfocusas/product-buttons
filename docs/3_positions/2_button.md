**Button**

![Button](images//button/button.png 'Button')
A button is the basic action handler you push it and something happens, it has a lot of properties, and we will go through them step by step.

The first ting to notice is the 8 dots in the top left corner of a selected button this is the *Handle bar* if you hover your mouse over it, it will change into an open hand, and you can click to grab the button and move it around the grid.

![Button properties 1](images/button/button_properties_1.png 'Button properties 1')
**Label** in the top right corner is the name of the button in the tree view.
**Style** is how the layout on the button will be presented.
* The first is a combination of an Icon and one line of text.
* The second is icon only.
* The third is 3 lines of text where the top line is color inverted.
* The fourth is 3 lines of text where the middle line is bigger than the others.

**Icon** will present you with a dropdown of multiple different icons, you can use search to find an appropriate icon.
![Icon](images/button/icon.png 'Icon')

![Button properties 2](images/button/button_properties_2.png 'button properties 2')
**Context** Is the top line in the Third and Fourth button style  
**Text** Is the middle line in the Third and Fourth button style and the only line in the First button style
**Text 2** Is the lower line in the Third and Fourth button style
all text lines can use plain text or `variables` where you can have dynamic content from connected equipment or from `Buttons` itself.
![Button properties 3](images/button/button_properties_3.png 'Button properties 3')
![Button variable](images/button/button_variable.png 'button variable') 
**Button styling**
![Button Properties 4](images/button/button_properties_4.png 'Button properties4')
![Button styling](images/button/button_styling.png 'Button styling')
**Location**
![Location](images/button/location.png 'Location')
`Flow` determine how a `Button` behave or are positioned relative to other elements in the grid

- `Float` Used to position an element in the first available slot, starting from top-left. The go-to for a dynamic layout.
- `Static` When you want full customization of where any button is placed. Set X / Y.
- `Anchor` Used to automatically position an element in any corner. Allows a section to be easily resized while keeping an element in any corner.
- `Fixed` Used to automatically position an element in any corner, but will not be affected by scrolling. (Sticky)
  
**Action**
![Action_1](images/button/action_1.png 'Action_1')
`Action` is where we connect the `Button` with `connections` or other functions inside `Buttons` itself. For this example we will use the button to perform a `Action` on a Blackmagic design Atem switcher. There are 5 action handlers to choose from 

- Down which will perform the action when you press the button.
- Up which will perform the action when you release the button.
- Left that will "move" the action to the `Encoders` on she `SDS` and perform the action when it's rotated left.
- Right that will "move" the action to the `Encoders` on the `SDS` and perform the action when it's rotated right.
- Encoder that will "move" the action to the `Encoders` on the `SDS` and perform a "-action" when turned left and a "+action" when turned right.
  
![alt text](images/button/action_2.png)  
For this example we will use the `Down` action handler 
![alt text](images/button/action_add_action.png)
`Click` on `+ Add Action` and chose an action from the popup menu this menu can be very extensive with a lot of `connections`. You can also`click` the ... menu to bring up a search and filter selection menu

![Action search](images/button/action_search.png 'Action search')
![Action search 2](images/button/action_search_2.png 'Action search 2')

Click on `ME:Set Program Input`

![Action 3](images/button/action_3.png 'Action 3')

We have now created a button that when pushed will set the Program bus on the Atem to input 1.

Let's jump back to the properties quickly and change the text on the button
![Button Atem Variable](images/button/button_variable_atem.png 'Button Atem Variable')
Notice that when you start typing the $ `Buttons` will start suggesting possibilities for you. Use a "." to separate the different parts of the variable.
![Button with variable](images/button/button_with_variable.png 'Button with variable')
Let's go back to the `Action` dialog
![Action dialog](images/button/action_1.png 'Action dialog')
There is more to this than first meets the eye notice the + sign between Step 1 and Feedbacks, by `Clicking` this you will add steps making the button a little "playlist" which will perform  one action after the other each time you press the button.
![Action 3](images/button/action_3.png 'Action 3') 
 You can also add more actions in the same step by pressing the `+ Add Action` at the bottom of the dialog. And add a delay from the press of the button to the action fires all delays are from the press of the button.
 But now we will look into the `Feedback` tab of the `Action` dialog
 ![Feedback dialog](images/button/feedback.png 'Feedback dialog')
 `Click` the `+ Add Feedback`
 ![Feedback 2](images/button/feedback_2.png 'Feedback 2')
`Click` on `ME: One ME Program source`this will bring up the following dialog.
![Feedback 3](images/button/feedback_3.png 'Feedback 3')
Here you will be presented with options to alter the text and style of the button if the choices in `Options` are True (or False if you use the invert button) in other words if Input 1 is chosen as the source on the ME one Program Bus
![Feedback 4](images/button/feedback_4.png 'Feedback 4')
Let's go into `Button Styling` and add a red background color. Now the button background will turn red every time Input 1 is live on the Program bus of M/E1.

If you have been following along in `Buttons` you may have noticed this dialog box popup every time you press the `Shift` button

![Execute mode](images/button/execute_mode.png 'Execute mode')
This will enable you to test your buttons without a surface connected. So hold `Shift` and `click`on a button to execute its actions.

There are a few more options in the properties list of buttons, but we will get back to them at a later stage. Now let's jump to a method that for many connections makes configuring a button much easier and much faster. `Presets`

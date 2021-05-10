#  Cell Setup

Open Main.storyboard and select the collection view in the Emoji Dictionary Scene. In the Attributes inspector, at the top, change Items from 0 to 1 to add a new item to the collection view. Click on the newly added cell (directly in the scene or via the Document Outline). At the top of the Attributes inspector, under Collection Reusable View, set the Identifier to Item.

Drag a label from the Object library to the new cell and change its text to “😀” and the font to System 24.0. Next, drag another label from the Object library and place it to the right of the first label. Set its text to “Name Label” and the font to Title 3. Drag one more label from the Object library and place it below the second label. Change its text to “Description Label” and the font to Subhead.

Select the Name Label and Description Label and, using the Embed In tool, embed them in a stack view. With the new stack view still selected, Command-click the emoji label to select it as well. Using the Embed In tool, embed the selected views in another stack view.

With the outermost stack view selected, add top and bottom constraints equal to 11. Add a leading constraint equal to 18 and trailing constraint equal to 20. Using the Attributes inspector, make sure Alignment and Distribution are both set to Fill and that the spacing is 8.

Select the vertical stack view inside the horizontal stack view and set the Alignment to Fill, Distribution to Fill Equally, and Spacing to 0.

To keep the emoji label and the vertical stack view from being separated, select the emoji label and, using the Size inspector, change the Horizontal Content Hugging Priority to 252. For storyboard purposes, select the cell and drag its right border so it is 400 points wide (the actual width of the item is calculated by the layout).

With the cell still selected, open the Identity inspector and change the class to EmojiCollectionViewCell. Switch to the Connections inspector and connect the outlets for nameLabel, descriptionLabel, and symbolLabel to their appropriate UI elements in the item.

Finally, using the Connections inspector, drag from the connector next to “selection” to the navigation controller on the storyboard. For the segue type, choose Present Modally.

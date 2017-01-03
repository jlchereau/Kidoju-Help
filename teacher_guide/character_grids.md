## Character Grids {#character-grids}

Let us do a 3x3 magic square as explained at [http://www.dr-mikes-math-games-for-kids.com/3x3-magic-square.html](http://www.dr-mikes-math-games-for-kids.com/3x3-magic-square.html).

In a 3x3 magic square:

*   All digits from 1 to 9 are used;
*   The sum of digits on each line, column and diagonal is 15.

We shall disclose two numbers to ensure a unique solution.

Create a new Kidoju quiz as explained at the beginning of the _Teacher Guide_ and add a Label as explained in the _Labels_ section.

To add a character grid to the stage, select (click) the **Character Grid** tool in the toolbox and click the stage. A new character grid is added to the page with a default size of 9*9, that is the size of a sudoku.

Expand the **Display attributes** collapsible panel of the tools pane.

Keep the . (dot) sign to **Blank** out cells like the black cells in crosswords, but we won’t use it here.

Keep the **Whitelist** 1-9 constituted of any numbers from 1 to 9\. Another possible whitelist is A-Z. The expected value is actually what you would put between square brackets to make a regular expression. The whitelist is the list of authorized characters in the grid. Any character that does not match the whitelist is discarded.

Click the **Layout** button and enter part of the grid as shown here below, then click the **OK** button.

Note: the whitelist does not apply to the Layout. You can have characters in the initial layout which are not whitelisted.

The cells you have filled with values in the initial layout are locked and cannot be changed when playing your Kidoju, which is shown by a grey background.

Select the text of the label displayed on the page for the **Question** property in the **Test logic** collapsible panel of the tools pane.

Keep the default value for the **Validation** algorithm and click the **Solution** button to edit the solution as reproduced here below:

Click **OK**, then click **Save** and **Play** your Kidoju.

Once the character grid is filled, click the **Submit** button to obtain the score and correction.

Click the **Edit** button to return to the _Editor_.
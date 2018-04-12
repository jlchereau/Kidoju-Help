## JavaScript custom validations {#javascript-custom-validations}

For even more complex custom validation rules, Kidoju offers the possibility to write your own code. For the security of our users:

*   Your code is sandboxed in a web worker which does not have access to the document object model and unsafe objects including xmlHttpRequest and localStorage are disabled;
*   Your code is limited to 1000 characters;
*   The execution of your code is limited to 100ms after which the web worker that runs your custom validation code is killed.

In the first example, you will validate that the value entered in a Textbox is between 100 and 110 inclusive.

Design your page as represented here below. After selecting the Textbox on the page, expand the **Display attribute** collapsible panel of the tools pane and add a **Mask** of 000 to constrain any user entry to 3 digits as explained in the _Textboxes_ chapter.

Then expand the **Test logic** collapsible panel of the tools pane and enter a **Question** and a **Solution** to be displayed in the score report. The solution will only be used as an example of correct value and will not be part of the validation algorithm.

Then click the **[…]** button corresponding to the **Validation** property to open the script editor. Teaching JavaScript is beyond the scope of this User Guise and we assume you have a basic knowledge of JavaScript programming.

Enter the following function:

function validate(value, solution, all) { return parseInt(value, 10) &gt;= 100 &amp;&amp; parseInt(value, 10) &lt;= 110;}

This function validates that the value entered parses as an Integer comprised between 100 and 110 included.

Click **OK**, then click **Save** and **Play** your Kidoju.

Note: Note that the solution is only given as an example and Kidoju validates a different value as a correct answer.
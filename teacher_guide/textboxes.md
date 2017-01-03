## Textboxes {#textboxes}

Textboxes are areas for typing text and provide short answers.

Add a third page as explained in the _Adding, removing, duplicating and sorting pages_ chapter. Add a label as explained in the _Labels_ chapter. Possibly add an image as explained in the _Images_ chapter using http://cliparts.co/clipart/1615\. Try to complete the following screenshot.

To add a textbox to the stage, select (click) the **Textbox** tool in the toolbox and click the stage. A new textbox is added to the page.

Then type “LLL” in the **Mask** property of the **Display attributes** collapsible panel of the tools pane. A mask of “LLL” constrains the answer to 3 letters and all other characters (digits and symbols) are discarded. Consider the mask as an optional hint.

A mask determines allowed characters and is made of the following rules:

| 0 | Digit | Accepts any digit between 0 and 9. |
| --- | --- | --- |
| 9 | Digit or space | Accepts any digit between 0 and 9, plus space. |
| # | Digit or space | Like 9 rule, but allows also (+) and (-) signs. |
| L | Letter | Restricts input to letters a-z and A-Z. This rule is equivalent to [a-zA-Z] in regular expressions. |
| ? | Letter or space | Restricts input to letters a-z and A-Z and to spaces. This rule is equivalent to [a-z A-Z] in regular expressions. |
| &amp; | Character | Accepts any character. The rule is equivalent to \S in regular expressions. |
| C | Character or space | Accepts any character. The rule is equivalent to . (dot) in regular expressions. |
| A | Alphanumeric | Accepts letters and digits only. |
| a | Alphanumeric or space | Accepts letters, digits and space only. |
| . | Decimal placeholder | The decimal separator will be get from the current culture. |
| , | Thousands placeholder | The display character will be get from the current culture. |

You might find the following examples useful

| Mask | Accepts | Rejects |
| --- | --- | --- |
| LLL | Abc | 123 |
| LL?LL | Ab cd | 123 |
| LL LL | Ab cd | 123 |
| 0000 | 1234 | 123 |
| 00-00 | 12-34 | 12-3 |

Resize the component bearing in mind the preceding chapter about _Position of correction ticks and crosses_.

Select the text of the label displayed on the page for the **Question** property in the **Test logic** collapsible panel of the tools pane.

Type “dog” in the **Solution** property.

Select “ignoreCaseEqual” for the **Validation** property. This validation algorithm ignores case and accepts “DOG”, “dog” and even “DoG” as correct answers.

Textboxes provide the following validation algorithms:

| equal | Strict comparison: résumé = résumé. |
| --- | --- |
| ignoreCaseEqual | Comparison ignoring case: RéSuMé = résumé. |
| ignoreCaseMatch | See the chapter about _Regular Expressions_ in the _Advanced Guide._ |
| ignoreDiacriticsEqual | Comparison ignoring case and diacritics: rEsUmE = résumé. |
| match | See the chapter about _Regular Expressions_ in the _Advanced Guide._ |
| metaphone | Phonetic comparison based on the metaphone algorithm: RAISUMER = résumé. |
| soundex | Phonetic comparison based on the soundex algorithm: RAISUMER = résumé. |

Note: more information on metaphone and soundex can be found at https://en.wikipedia.org/wiki/Phonetic_algorithm. These algorithms work best in English and soundex is more permissive than metaphone.

Keep default values for the **Success**, **Failure** and **Omit** points.

Note: do not forget to save your work often.

After clicking the **Save** button, **Play** your Kidoju.

Click the **Edit** button to return to the _Editor_.
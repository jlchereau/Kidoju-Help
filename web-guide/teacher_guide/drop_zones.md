## Drop zones {#drop-zones}

Drop zones provide a surface to drop images and/or labels and validate their value.

Add a fifth page as explained in the _Adding, removing, duplicating and sorting pages_ chapter. Add a label as explained in the _Labels_ chapter. Add two image as explained in the _Images_ chapter using http://cliparts.co/clipart/23725 and http://cliparts.co/clipart/3120348\. Try to complete the following screenshot.

Duplicate the fish images by clicking the menu handle and selecting the **Duplicate** option as shown above. Then define the test logic on each fish by turning draggable on and assigning a value of 1\. The drop zone will ensure that the user will have dropped 1 + 1 = 2.

To add a drop zone to the stage, select (click) the **Drop Zone** tool in the toolbox and click the stage. A new drop zone is added to the page with a dashed border and a “Please drop here” invitation which you can change.

IMPORTANT! Sort your drop zone and draggable images and labels in the page explorer so that all draggable images are listed at the bottom, just after the drop zone. The reason is you want draggable images on top of everything else.

Select the text of the label displayed on the page for the **Question** property in the **Test logic** collapsible panel of the tools pane.

Type “2” in the **Solution** property.

Select “sumEqual” for the **Validation** property.

Textboxes provide the following validation algorithms:

| equal | Strict comparison: résumé = résumé. |
| --- | --- |
| sumEqual | Comparison ignoring case: RéSuMé = résumé. |

Note: more information on metaphone and soundex can be found at https://en.wikipedia.org/wiki/Phonetic_algorithm. These algorithms work best in English and soundex is more permissive than metaphone.

Keep default values for the **Success**, **Failure** and **Omit** points.

Note: do not forget to save your work often.

After clicking the **Save** button, **Play** your Kidoju.

Click the **Edit** button to return to the _Editor_.
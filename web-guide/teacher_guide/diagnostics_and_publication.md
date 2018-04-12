## Diagnostics and publication {#diagnostics-and-publication}

Now, let us suppose your test is ready for publishing. Click the **Publish** button.

Assuming you have followed the instructions in this User Guide, you should get the following error message:

Discarding the error message by clicking the **OK** button reveals the Diagnostic Console with warnings and errors.

In this instance, you have 10 warnings and 1 error. Warnings (in yellow) are recommendations which do not prevent from publishing. Errors need to be fixed before publishing.

Amongst warnings, the software recommends adding _User instructions and explanations_ on all pages. Simply click a warning in the Diagnostic Console to navigate to the corresponding page and make the required correction.

There should only be one error: “At least 10 questions are required to be allowed to publish”. Each component has a weight:

*   _Labels_ and _Images_ have a weight of 0: they do not make questions;
*   _Quizzes (or multiple choice questions)_, _Checkboxes_ and _Textboxes_ have a weight of 1, as each of them make a question;
*   _Connectors_ have a weight of 0.25, as we consider you need at least 4 connectors to make a question;
*   _Character Grids_ have a weight of 10, as any grid would require several cells to fill, constituting several questions.

In order to prevent the publication of unfinished user trials, we require that Kidoju quizzes you publish have at least 10 questions, i.e. that the sum of all weights from all page components is at least 10.

Note: “with great power comes great responsibility”. Please be responsible and only publish contributions you are proud of and keep your trials as private drafts.
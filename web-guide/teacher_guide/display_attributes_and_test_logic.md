## Display attributes and test logic {#display-attributes-and-test-logic}

We have divided the properties of a component into display attributes which affect the way components are displayed and test logic which affect the way they contribute to the score of a knowledge test.

### Display attributes {#display-attributes}

Display attributes essentially include position, size and style. Currently all components have display attributes.

In particular, image, audio and video components designate files which you can upload to our servers. There is currently a limit to the size of uploaded files and you might get an error if the file you are trying to upload is too big. There are good reasons to limit the size of files specially to protect mobile device users consuming knowledge tests on 3G data plans.

Note: there are many free tools to crop and resize images including Paint on Windows® and the image previewer on macOS®.

### Test logic {#test-logic}

Components which participate in the answer to a question have test logic properties. Test logic generally comprises a question and a solution displayed in the score grid, a validation rule and points to compute the final score.

A validation rule can be a predefined algorithm or a custom function. The most common predefined algorithm is “equal” which compares the answer value with the solution value.

Note: more on custom functions in the JavaScript custom validations chapter of the Advanced Guide.

There are points (including negative points) for successfully answering, failing to answer correctly and omitting to answer.

The following screenshot shows how these fields are displayed in the score grid.
## Regular Expressions {#regular-expressions}

The “match” and “ignoreCaseMatch” validation algorithms of _Textboxes_ use regular expressions to validate a user answer typed in a textbox.

Regular expressions are extensively documented at [http://www.regular-expressions.info/](http://www.regular-expressions.info/) and this chapter can only be considered an introduction. We recommend that you test your regular expressions at [http://www.regexr.com/](http://www.regexr.com/).

The /i option at the end of the regular expression “^napol[eé]on$” corresponds to “ignoreCaseMatch”. It matches both “napoleon” and “NAPOLEON”.

^ and $ are anchors which work has follows:

*   The regular expression “napoleon” matches any value that contains the word “napoleon”.
*   The regular expression “^napoleon” matches any value that starts with the word “napoleon”.
*   The regular expression “napoleon$” matches any value that ends with the word “napoleon”.
*   The regular expression “^napoleon$” only matches the exact word “napoleon”.

[eé] matches any character in the set delimited by square brackets. In this case, [eé] matches both “e” and “é”. Accordingly, “^napol[eé]on$” matches both “napoleon” and “napoléon”.

[a-z] matches any alphabetical character from a to z.

[0-9] matches any digit from 0 to 9.

[a-z]{2} matches any combination of exactly 2 alphabetical character from a to z. Therefore [a-z]{1} is equivalent to [a-z].

[0-9]{2,4} matches any combination of 2 to 4 digits.

[a-z]* matches 0 or more alphabetical characters.

[a-z]+ matches 1 or more alphabetical characters.

[a-z0-9A-Z_], that is any alphabetical character (lower case or upper case) or any digit or underscore can be shortened as \w.

^(napol[eé]on|bonaparte)$ matches both NapOléOn and BOnApArte.

Because a dash (-) designates a range, dashes need to be escaped as \- in regular expressions. The same applies to square brackets and dollar signs which need to be escaped respectively as \[, \] and \$ if used literally in regular expressions.

\s is used to match a space, a tab (\t) or a line feed (\n).

We are only scratching the surface to get you started. Regular expressions are extremely powerful and allow complex validations without writing any programming code.
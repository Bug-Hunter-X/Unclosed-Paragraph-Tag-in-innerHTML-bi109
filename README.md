# Unclosed Paragraph Tag in innerHTML

This repository demonstrates an uncommon bug in HTML related to using `innerHTML` to modify existing content. The issue arises from an unclosed paragraph tag within the string assigned to `innerHTML`.  This can lead to unpredictable rendering behavior in different browsers, especially concerning the display of elements following the malformed tag.

**Bug:** The main bug lies in how the `innerHTML` is set for the `div` with id "myDiv".  The first paragraph is correctly opened and closed but the second paragraph is missing a closing tag. This omission causes rendering issues and potential layout problems.

**Solution:** Correctly close all the HTML tags within the string to be used as the `innerHTML`.  A well-formed HTML string should have matching opening and closing tags.
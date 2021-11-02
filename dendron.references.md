---
id: m6czSj5gQzAdGJHUWW4pS
title: References
desc: ''
updated: 1635817009630
created: 1635816954122
---

## Note references

https://wiki.dendron.so/notes/f1af56bb-db27-47ae-8406-61a98de6c78c/

## Summary

Dendron allows you to reference content from other notes and embed them in your current note. This is also known as transclusion.

Note references are different from regular links in that they actually include the content of the destination in the current note.

Note references are extremely powerful and help you re-use your notes in a variety of places.

Currently, Dendron supports 4 types of references to help you control the amount of content that gets embedded:

full note references
header references
block references
range references
References have the following syntax:

![[name.of.note]]
Here's an example with a block anchor:

![[name.of.note#^important-paragraph]]
Another example with a header range:

![[name.of.note#starting-header:#ending-header]]
NOTE: When referencing headers with spaces in them, the note ref needs to use - instead of spaces within the name. This is a limitation of adopting GitHub-style slugger references. This is also useful for when multiple subheaders on a page may have the same name, which would expect something else #foo vs. #foo-1 vs. #foo-2. This can be automatically taken care of by highlighting a header, and using cmd+shift+r / ctrl+shift+r to add a properly-formatted note ref to the clipboard.

For more information:

StackOverflow: How to escape symbols in GitHub-flavored markdown internal links / heading anchors?
Anchors in Markdown gist

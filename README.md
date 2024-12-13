# events-calendar-bug-18195987

The Events Calendar 6.8.3
WordPress Version 6.7.1
Theme: Twenty Twenty-Five

## Description

The issue relates to the unexpected insertion of your ian-client into the Gutenberg editor.

## Reproduce

1. Add a new event.
2. Insert the Post Title block (core/post-title) and set it to level 1.
3. Add a paragraph block after the level 1 Post Title.
4. Save the editor and refresh the page. It crashes when inserting another block.

![Bug](./events%20calendar.gif)

Error:

`NotFoundError: Failed to execute 'insertBefore' on 'Node': The node before which the new node is to be inserted is not a child of this node.`

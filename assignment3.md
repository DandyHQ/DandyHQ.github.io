### Improvements already made

* Arrow keys now work
* Pressing Enter retains indentation level
* Undo and Redo have been implemented
* Multiple cursors
* Replaced a large amount of Lua with a small amount of C
* Fixed bug where Mace would sometimes crash when the save commands was used
* Config file allows customisability (font, scrollbar, key bindings)
* The usual keyboard bindings (reconfigurable)
* Acme style scrollbar
* Rendering has been revamped such that Mace is faster now

### Things to Improve

* Cut, Copy and Paste don't work with the system paste buffer
* Reimplement tiles
* Goto line number
* Various bug fixes and bits of polish

### Schedule for remaining work

?????

## Actual Assignment

<some sort of good introduction>

Changes we've done already:


Mace was not entirely finished at the end of semester 1, so we already had some ideas about what still needed to be implemented or fixed. After using Mace for our text editing needs during the break and this semester, we have been able to see more ways in which the product can be further improved. 
One of the glaring problems for Mace's usability was that the arrow keys did nothing, making it more difficult to navigate the text. We have now implemented this, and spent time to ensure that this works completely and intuitively, with any UTF-8 characters. Additionally, Mace now has keyboard shortcuts for various commands (cut, paste, save, etc), and new Undo/Redo commands have been added.
One of the core design principles behind Mace is that the user should be able to customise the text editor to suit their preferences. Mace now has a config file, where the user can change keybindings for commands, the position and behaviour of the scrollbar, and the font.

etc etc

Changes we're gonna do:

We originally intended for Mace to have a "malleable" user interface, in which the window would be separated into resizable, rearrangeable tiles. This would allow the user to keep multiple files in view at once, at minimal cost of screen space. Unfortunately, this feature was not included in our semester 1 deliverable due to time constraints. We intend to reimplement this feature this semester.
Another problem is that Cut, Copy and Paste commands do not work with the system paste buffer. 

Scheduling:

To improve the usability of Mace this semester, we will make the above changes (and do some polishing / bug fixing). Here is the schedule we are going to use:
[something]

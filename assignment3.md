### Improvements already made

*  Arrow keys now work
*  Pressing Enter retains indentation level
*  Undo and Redo have been implemented
* Multiple cursors
* Replaced a large amount of Lua with a small amount of C
*  Fixed bug where Mace would sometimes crash when the save commands was used
*  Config file allows customisability (font, scrollbar, key bindings)
*  The usual keyboard bindings (reconfigurable)
* Acme style scrollbar
* Rendering has been revamped such that Mace is faster now

### Things to Improve

*  Cut, Copy and Paste don't work with the system paste buffer
*  Reimplement tiles
* Goto line number
*  Various bug fixes and bits of polish

### Schedule for remaining work

?????

## Actual Assignment

<some sort of good introduction>

Changes we've done already:


Mace was not entirely finished at the end of semester 1, so we already had some ideas about what still needed to be implemented or fixed. After using Mace for our text editing needs during the break and this semester, we have been able to see more ways in which the product can be further improved. 

One of the glaring problems for Mace's usability was that the arrow keys did nothing, making it quite difficult to navigate the text. We have now implemented this, and spent time to ensure that this works completely and intuitively, with all UTF-8 characters. Additionally, Mace now has familiar keyboard shortcuts for various commands (cut, paste, save, etc), and new Undo/Redo commands have been added. We have also fixed a bug that our marker pointed out: that Mace would sometimes crash when the save commands were used.

Remove Lua and replace with C, revamped rendering.

When using Mace, we found that it was annoying that it didn't retain the current indentation level when Return was pressed, but it went to the start of the next line. We have since implemented this feature, and also plan to implement block indenting and block unindenting, meaning that the user can highlight a block of text and change the indent level of all of it at once.

Acme style scroll bar and multiple cursors

One of the core design principles behind Mace is that the user should be able to customise the text editor to suit their preferences. Mace now has a config file, where the user can change keybindings for commands, the position and behaviour of the scrollbar, and the font.

Changes we're gonna do:

We originally intended for Mace to have a "malleable" user interface, in which the window would be separated into resizable, rearrangeable tiles. This would allow the user to keep multiple files in view at once, at minimal cost of screen space. Unfortunately, this feature was not included in our semester 1 deliverable because we underestimated how much time it would take to get everything done. We intend to reimplement this feature this semester.

Another problem is that cut, copy and paste commands do not work with the system paste buffer, which means that text cannot be copied and pasted in or out of Mace from or to other applications. This is something that we didn't realise we use as much as we do, but trying to use Mace as our primary text editor showed us that it is an important feature, so we are aiming to have that implemented by the end of the semester as well.

Goto line number

Scheduling:

To improve the usability of Mace this semester, we will make the above changes (and do some polishing / bug fixing). Here is the schedule we are going to use:


#### PROJECT MANAGEMENT

Task | Timeframe | Project Member/s
--- | --- | ---
Get arrow keys to work | DONE | Ryan/Hannah/Mytchel
Pressing Enter retains indentation level | DONE | Mytchel
Undo and Redo have been implemented | DONE | Mytchel
Multiple cursors | DONE | Mytchel
Replaced a large amount of Lua with a small amount of C | DONE | Mytchel
Fixed bug where Mace would sometimes crash when the save commands was used | DONE | Mytchel
Config file allows customisability (font, scrollbar, key bindings) | DONE | Mytchel
The usual keyboard bindings (reconfigurable) | DONE | Mytchel
Acme style scrollbar | DONE | Mytchel
Rendering has been revamped such that Mace is faster now | DONE | Mytchel
Get cut, copy and paste to work with the system paste buffer | 2 weeks (28 Aug) | Mytchel 
Reimplement tiles | 2 weeks (11 Sept) | Mytchel
Goto line number | 2 weeks (25 Sept) | Mytchel
Various bug fixes and bits of polish, ready to submit | 1 week (2 Oct) | Mytchel

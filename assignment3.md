## Assignment 3

After using Mace for our text editing needs during the break and this semester, we have been able to see many ways in which the product can be further improved. Mace was not entirely finished at the end of semester 1, so we already had some ideas about what still needed to be implemented or fixed. Using it gave us some ideas for further improvements.

One of the glaring problems for Mace's usability was that the arrow keys did nothing, making it quite difficult to navigate the text. We have now implemented this, and spent time to ensure that the arrow keys work completely and intuitively, with all UTF-8 characters. Additionally, Mace now has familiar keyboard shortcuts for various commands (cut, paste, save, etc), and new Undo/Redo commands have been added. We have also fixed a bug that the marker of our semester 1 deliverable pointed out: that Mace would sometimes crash when the save command was used.

In semester 1, we used Lua for font initialisation and commands (e.g. cut, copy, save). However, we found that this was not as useful as we had expected, and required a very large amount of code for relatively minor tasks. We have since replaced this with a smaller amount of C. We have also changed the way that Mace renders text, such that the application runs faster overall. For example, Mace now only renders entire lines - that is, if a line at the top or bottom of the window cannot fit vertically, it will not be rendered.

When using Mace, we found that it was annoying that the cursor didn't retain its current indentation level when Return was pressed. Rather, it just went to the start of the next line. We have since fixed this. We also plan to implement block indenting and unindenting, meaning that the user can highlight a block of text and change the indent level of all of it at once.

Since semester 2, we have implemented some features that we have seen in other text editors that are useful but not widely available. For example, Mace now supports the use of multiple cursors. By middle-clicking, the user can create additional cursors, which all function the same way. This can be helpful for adding or editing the same snippet of code in multiple places at once. Left-clicking moves the cursor and removes all additional cursors. We have also switched to an Acme-style scrollbar, where different mouse buttons can have different effects when the scrollbar is clicked. By default, left-clicking the scrollbar scrolls up, right-clicking scrolls down, and middle-clicking scrolls directly to the position corresponding to where the scrollbar was clicked. In the first two cases, clicking near the top of the bar scrolls a little bit, while clicking near the bottom scrolls a lot.

One of the core design principles behind Mace is that the user should be able to customise the text editor to suit their preferences. Mace now has a config file, where the user can change the font and keybindings for commands. The behaviour and position of the scrollbar are also configurable now. Understanding that some users prefer the scrollbar on the left, closer to the majority of the text, we have added this as an option in the config file. The behaviour of the different mouse buttons, as described above, is also customisable in this way.

We originally intended for Mace to have a "malleable" user interface, in which the window would be separated into resizable, rearrangeable tiles. This feature was not included in our semester 1 deliverable because we underestimated how much time it would take to get everything working together. After using Mace since then, we have decided that this feature is not important for the fundamental usability of Mace, and therefore we will not try to reimplement it.

When editing and debugging code, it is important to be able to easily find the line where an error occurs. This became apparent to us very quickly when coding with Mace. To this end, we have added a "goto" command, which allows the user to jump directly to a line of code by its number (e.g. the number given by compiler error messages). At this point, this command moves the cursor to the appropriate location. We intend to also have the window scroll to this point.

A remaining problem with Mace is that the cut, copy and paste commands do not work with the system paste buffer, which means that text cannot be copied and pasted in (or out) of Mace from (or to) other applications. This is something that we didn't realise we use as much as we do, but using Mace as our primary text editor showed us that it is a very important feature. We are aiming to have that implemented by the end of the semester.

#### PROJECT MANAGEMENT

To improve the usability of Mace this semester, we will make the above changes (and do some polishing / bug fixing). Here is the schedule we are going to use:

Task | Timeframe | Project Member/s
--- | --- | ---
Pressing Return retains indentation level | DONE | Mytchel
Undo and Redo have been implemented | DONE | Mytchel
Multiple cursors | DONE | Mytchel
Get arrow keys to work | DONE | Ryan, Hannah, Mytchel
Replaced Lua with C | DONE | Mytchel
Fixed bug where Mace would sometimes crash when the save commands was used | DONE | Mytchel
Config file allows customisability (font, scrollbar, key bindings) | DONE | Mytchel
The usual keyboard bindings (reconfigurable) | DONE | Mytchel
Acme-like scrollbar behaviour | DONE | Mytchel
Left-hand side scrollbar option | DONE | Vaughan
Improve rendering | DONE | Mytchel
Block indenting | 21 Aug | Ryan, Hannah
Go to line number (with scrolling) | 28 Aug | Vaughan
Page Up/Down | 28 Aug | Ryan, Hannah, Vaughan
Get cut, copy and paste to work with the system paste buffer | 4 Sept | Mytchel
Final round of bug fixing / polish | 2 Oct | Everyone

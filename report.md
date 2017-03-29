### 345 Report Draft

> ##### Basic specifications
> * describe what we're building
> * explain "who is going to build it", i.e. who's doing what, I guess
> * explain how we're going to ensure quality of source code and product
> * say how long it's going to take to build
> * explain why we're gong to use the software every week

#### SECTION ONE: WHAT AND WHY

A text editor is a crucial tool in the belt of any software engineer. While text editors all share a set of fundamental features (namely, the ability to create, edit and delete plain text files), different editors vary considerably in what they have to offer. For example, notepad is certainly a text editor, but lacks many features that a software engineer might consider essential. We plan to build a text editor that fulfills these common necessities and also includes some features that are often omitted by similar pieces of software. In particular, we aim to capture the power of emacs and the UI versatility of acme (hence the name, Mace).

One of the core principles behind the design of Mace is that the user should be able to configure the text editor however they want. This means that we want to have a malleable user interface. In our design, the window is separated into tiles. These tiles can hold multiple tabs and can be arranged either horizontally or vertically from each other. This way, the user can keep multiple files in view at once at minimal cost of screen space.

Additionally, Mace will have an editable action bar, from which the user can quickly execute common commands like Cut, Paste and Find. It will be possible to remove/add commands to the bar by simply clicking and typing their names in. They can then be executed by middle-clicking on them. A basic set of commands will be recognised by default, but there will also be support for custom commands via an extension language.

We also intend for Mace to be able to browse directories and edit streams.

These features are the ones we consider to be fundamental to our product. Once they are implemented we plan to look at adding other common features of text editors, such as syntax highlighting, smart indenting and keyboard shortcuts, as well as some less common features like multiple cursors and the ability to undo operations beyond the scope of text editing (e.g. window movements, file changes).

Mace is intended to work on all Unix systems and OSX.

#### SECTION TWO: WHO AND HOW

Our group is quite diverse with respect to areas of expertise. As the best programmer, Mytchel is the lead programmer for the project. Vaughan has taken on the design and prototyping, and will also be programming. Hannah and Ryan have less experience programming, but will be contributing in small ways to the source code where possible - mainly, they will be responsible for project tracking, scheduling, reviewing, etc. Naturally, we will all be testing the product through use, once it has reached a usable state.

The integrity of the code will be supported through version control (via GitHub) and continuous integration. We will be testing the software both through use and with custom software tests.

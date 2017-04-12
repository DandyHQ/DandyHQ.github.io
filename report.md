### COSC345 Report 1

#### SECTION ONE: WHAT AND WHY

A text editor is a crucial tool in the belt of any software engineer. While text editors all share a set of fundamental features (namely, the ability to create, edit and delete plain text files), different editors vary considerably in what they have to offer. For example, notepad is certainly a text editor, but lacks many features that a software engineer might consider essential. We plan to build a text editor that fulfills these common necessities and also includes some features that are often omitted by similar pieces of software. This text editor takes several points of inspiration from emacs and acme, and will be called Mace.

One of the core principles behind the design of Mace is that the user should be able to configure the text editor however they want. This means that we want to have a malleable user interface. In our design, the window is separated into panes. These panes are resizable, can hold multiple tabs, and can be arranged either horizontally or vertically from each other. This way, the user can keep multiple files in view at once at minimal cost of screen space. Each pane can be used to view and edit text files, or to browse directories.

Mace will also have an editable action bar, from which the user can quickly execute common commands like Cut, Paste and Find. It will be possible to remove/add commands to the bar by simply clicking and typing their names in. They can then be executed by right-clicking on them. A basic set of commands will be recognised by default, but there will also be support for custom commands via an extension language (Lua). We have created some [initial designs](https://github.com/DandyHQ/mace-design) of the UI to get us started and make sure that everyone has the same idea about what we want it to look like.

These features are the ones we consider to be fundamental to our product. Once these goals have been reached, we plan to look at adding other common features of text editors, such as syntax highlighting, smart indenting and keyboard shortcuts. Mace is intended to work on ubuntu, openBSD and fedora.

#### SECTION TWO: WHO AND HOW

Our group is quite diverse with respect to areas of expertise. As the most experienced coder, Mytchel is the lead programmer for the project. Hannah and Ryan have less experience programming, but will be contributing to the source code in smaller ways wherever possible. Mainly, they will be responsible for project tracking, scheduling and reviewing. Vaughan has taken on the role of lead designer for the project, and will also be programming.

We will be using a number of libraries to support the implementation of Mace. These include Xlib, for the main display of the application, freetype2 for managing font files, and utf8proc for UTF-8 handling. Lua will be used for the implementation of the commands on the command bar. We have also decided to use the Meson build system instead of Make. While Meson is a little less portable than Make, we think that it will ultimately be easier to work with, because it is fast, easy to read, and it will make testing easier down the road.

The integrity of the code will, of course, be supported by version control through GitHub. Additionally, we will be using the Unity testing framework to set up automated tests of the code, and we will all use the product once it has reached a working state, in order to test it from a user perspective. Early in development, we discussed writing our own libraries with a consistent error interface for improved debugging. However, we eventually decided that this would be unnecessary and too time-consuming. We also discussed using a garbage collector, but ultimately decided that this would likely reduce the responsiveness of the application.

We also plan to be vigilant with our documentation, to best enable smooth collaboration. Mytchel has made this [development document](https://github.com/DandyHQ/mace/wiki/Development) for reference, and we are all committed to producing clear, informative and regularly updated comments in the code where necessary. We also have regular (weekly) meetings to touch base, discuss any issues we're having, and make clear plans about what each of us will do over the following week. Ryan takes minutes at each meeting, and these are [all available](https://github.com/DandyHQ/DandyHQ.github.io/tree/master/minutes) on GitHub for the team's reference.

Another way we are trying to ensure the quality of our product is through prototyping. Vaughan has created an [interactive prototype](https://github.com/DandyHQ/mace-prototype) of Mace's UI, so that we all have something to refer to when building the source code. This way, we are less likely to inadvertently weaken the design to make the work easier during implementation.

#### PROJECT MANAGEMENT

Task | Timeframe | Project Member/s
--- | --- | ---
Key features selected | Done | All
Github repository created, all members added | Done | All
Tentative schedule created | Done | Hannah/Ryan
**Deliverable** Report 1 | Done | Ryan/Hannah
Designs of the UI drawn up | Done | Vaughan
Prototype of the basic functions | Done | Vaughan
Windows and panes (within windows) can be created | Done | Mytchel
Panes can be dragged to split the window | Done | Mytchel
Text can be entered | Done | Mytchel
Action Bar is editable | Done | Mytchel
Panes can be resized | 1 week | Ryan
Font can be selected and changed | 2 weeks | Hannah
Basic commands can be executed (copy/paste/save/find etc) | 1.5 weeks | Mytchel/Vaughan
Changes recorded, undo can be executed | 1.5 weeks | Mytchel/Vaughan
Custom commands can be created and executed | 2 weeks | Mytchel/Vaughan
Syntax highlighting | Merely desirable | ?
Smart indenting | Merely desirable | ?
Keyboard shortcuts | Merely desirable | ?

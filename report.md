### 345 Report Draft

> ##### Basic specifications
> * describe what we're building
> * explain "who is going to build it", i.e. who's doing what, I guess
> * explain how we're going to ensure quality of source code and product
> * say how long it's going to take to build
> * explain why we're gong to use the software every week

#### SECTION ONE: WHAT AND WHY

A text editor is a crucial tool in the belt of any software engineer. While text editors all share a set of fundamental features (namely, the ability to create, edit and delete plain text files), different editors vary considerably in what they have to offer. For example, notepad is certainly a text editor, but lacks many features that a software engineer might consider essential. We plan to build a text editor that fulfills these common necessities and also includes some features that are often omitted by similar pieces of software. This text editor takes several points of inspiration from emacs and acme, and will be called Mace.

One of the core principles behind the design of Mace is that the user should be able to configure the text editor however they want. This means that we want to have a malleable user interface. In our design, the window is separated into panes. These panes are resizable, can hold multiple tabs, and can be arranged either horizontally or vertically from each other. This way, the user can keep multiple files in view at once at minimal cost of screen space. Each pane can be used to view and edit text files, or to browse directories.

Mace will also have an editable action bar, from which the user can quickly execute common commands like Cut, Paste and Find. It will be possible to remove/add commands to the bar by simply clicking and typing their names in. They can then be executed by right-clicking on them. A basic set of commands will be recognised by default, but there will also be support for custom commands via an extension language. 

These features are the ones we consider to be fundamental to our product. Mace is intended to work on ubuntu, openBSD and fedora. 
Once these goals have been reached, we plan to look at adding other common features of text editors, such as syntax highlighting, smart indenting and keyboard shortcuts, as well as some less common features like multiple cursors and the ability to undo operations beyond the scope of text editing (e.g. window movements, file changes). *maybe we shouldn't be talking about future features, since that's the point of the second report? Might remove/replace this bit*

#### SECTION TWO: WHO AND HOW

Our group is quite diverse with respect to areas of expertise. As the most experienced coder, Mytchel is the lead programmer for the project. Hannah and Ryan have less experience programming, but will be contributing to the source code in smaller ways wherever possible. Mainly, they will be responsible for project tracking, scheduling and reviewing. Vaughan has taken on the role of lead designer for the project, and will also be programming.

The integrity of the code will, of course, be supported by version control through GitHub. Additionally, we will be using the Unity testing framework to set up automated tests of the code, and we will all use the product once it has reached a working state, in order to test it from a user perspective. Early in development, we discussed writing our own libraries with a consistent error interface for improved debugging. However, we eventually decided that this would be unnecessary and too time-consuming. We also discussed using a garbage collector, but ultimately decided that this would likely reduce the responsiveness of the application.

Another way we are trying to ensure the quality of our product is through prototyping. Vaughan has created an interactive prototype of Mace's UI, so that we all have something to refer to when building the source code. This way, we are less likely to inadvertently weaken the design to make the work easier during implementation.


# Roadmap
![MacVim](https://dl.dropbox.com/u/3684640/macvim/window.png)

Below is a rough roadmap, listing the items I would like to add and remove from
MacVim. The philosophy behind this redesign is simply to make the experience of
using Vim on a Mac as enjoyable and native-feeling as possible. In the end, this
project is about creating the editor I've always wanted. Hopefully it will
benefit others as well.

*Note: none of the screenshots reflect the current state of the app... they are just mockups*

## Toolbar
I never use it, so I'm going to remove it.

## Tabs (bufferlist)
PSMTabBar has served many projects well, but a horizontal row of tabs doesn't
fit well in my workflow. After using Espresso.app and Chocolat.app (which will
heavily influence this project), I have concluded that a "tab list" in the
sidebar is the most natural and unobtrusive placement for such a UI. This design
allows for the buffer listing to be hidden altogether (when hiding the file
browser), which is very nice when concentrating on a single file.

You should be able to reorder and close the items in the tab list, (I will refer
to it as a "bufferlist" from here on out).

## File browser (sidebar)
As you can see from the screengrab above, the project sidebar (I will refer to
it as the "sidebar" from here on out) will look and function like a traditional
OS X source list.

You should be able to drag files to and from the list, create/delete/rename
files and directories, "Open Finder here", "Open Terminal here", etc.

## Quick open
![MacVim - Quick Open](https://dl.dropbox.com/u/3684640/macvim/quick_open.png)

As it stands, there is no out-of-the-box quick open functionality in MacVim (by
quick open, I am referring to something similar to TextMate's cmd+t or
Chocolat's cmd+d). There are great Vim plugins like ctrlp, but I want to have a
native feeling UI for this action.

The quick open filter will appear "inline" in the sidebar to help keep our
window count down (no need to create a whole new window for a filtering process
that is directly related to the existing source list view...). This design is
borrowed from Espresso.app, but will vastly improve upon the concept.

## Path control
The header for the sourcelist will double as a "project root chooser", allowing
you to choose your working directory.

## Find/replace
![MacVim - Find](https://dl.dropbox.com/u/3684640/macvim/find.png)

The find and replace interface will move from a new window, to an inline design
inspired by Espresso.app and Chocolat.app. Of course this is just a nice bit of
UI for those uncomfortable with Vim's substitute command.

## Project find
![MacVim - Project Find](https://dl.dropbox.com/u/3684640/macvim/project_find.png)

Ack is great, but nothing beats a native feeling interface for searching a
project directory. This UI takes a stab at keeping even complex peripheral views
contained in one window, to reduce "cmd+~ induced cramps". It strives to keep a
connection between the search results and document.

---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

# Computer Networks and Control Systems KF5011

# reading list
Some suggested texts:

* Lee & Varaiya _Structure and Interpretation of Signals and Systems_ http://leevaraiya.org/
* Lee & Seshia _Introduction to Embedded Systems_ http://leeseshia.org/

Both books are available from their websites as PDFs (though it is nice having a hard-copy in hand [ludite that I am])

Also some O'Reilly books I've found useful

* Catsoulis _Designing Embedded Hardware_.  Good for material on the electronic interfacing side.
* Barr & Massa _Programming Embedded Systems_.  Based on using the GNU toolset
* White _Making Embedded Systems_.  Covers some more general aspects, state-machines etc.

The O'Reilly texts go with AVR (Arduino Uno) or other low cost systems, so we may have to be selective.

# Development platform

The [Atom](http://atom.io) editor is available for Windows, Linux, and Mac's.  By itself it has good support for programming.   The plugin/extension [PlatformIO](http://platformIO.org) adds specific support for embedded systems.  These make a good pairing, are freely available (Open-source), and I've successfully build code for the current ARM boards (as long as you avoid the Embedded artists library `EALib`), and Arduino Uno.  Using both C and assembly language.

# Course structure
We have a 12 week semester, with 2 hours of lectures and 2 hours of labs each week.  Based on feedback from the current students I'm going for a 2hour long lab session, and 2 seperate 1 hour lectures.

# AntiGo - the next big small desktop thing?

First, and above all: the LXQt desktop environment is nice, very nice. LXQt is written in C++, using the Qt graphical toolkit. 

It is a very complete, under estimated desktop! I find the result overwhelming and phenomenal nice. "It's a beauty". 

Anyway, after using another desktop, the FyneDesk desktop environment, for a while, and especially after enjoying the simplicity of its codebase, 
the idea came up to replace the lxqt-panel application (which is at the heart of LXQt) by something else. 
Although being a nascent idea, realisation was recently prompted by a novel change in LXQt 2.2, where multiple sessions of a desktop for the same user have been disabled. 

What a stupid design change!

Re-enabling this is simple (if you tweak the source a bit), and is OK for me. 
However, it fueled the forementioned idea, more specifically to re-implement parts of LXQt in the combination of Go and Fyne. Fyne is a graphical toolkit written in Go. 

History reveals that LXQt is, at it root, based on a project called "Antico" (which in turn was inspired by "QLWM"). The name of this derived project "AntiGo" was born rapidly.

My idea is just to replace "lxqt-panel", and create a drop-in "ntgo-panel" application. Once this new panel is functional, the chosen approach allows for gradual replacement of other parts of LXQt as well (if needed). Certain parts of LXQt (like qterminal, pcmanfm-qt) certainly do not need a retrofit!

Ambitious? Sure. 

For now, development takes place in a private repository. 

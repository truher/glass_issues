# Glass issues demo

Show stuff that doesn't work in glass, to make fixing it easier.

https://www.chiefdelphi.com/t/sim-glass-gui-state/446006/2


Steps to get here:

* download 2024.1.1-beta3 for linux
* create a new java project using the robotbase template
* modify .gitignore to allow checking in the window.json files
* start the glass tool -- it won't have much interesting in it
* move some things around, make a plot window
* save as global
* close glass
* open glass again
* the plot window is gone

Another experiment:

* click "simulate robot" with the simgui
* add a plot, move some things around.
* change the zoom level
* add a keyboard joystick
* save as global
* close the simulation
* the details are in the simgui.json file, including zoom level
* run it again
* the zoom level is reset
* the plot is gone
* the simgui.json file is rewritten

Another experiment:

* run glass and the simgui at the same time (as above)
* try "save as global" from glass
* add a plot to glass, plot the StationNumber
* the "save as global" is greyed out.
* try "save as," find a folder; the json file is correct now
* now the "save as global" is clickable
* close glass
* restart it
* open the thing that was saved
* nothing is retained.  the glass.json file is now empty.
* the window.json file is reset to its initial state
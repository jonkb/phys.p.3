------------------------------------------------------------------------
This is the project README file. Here, you should describe your project.
Tell the reader (someone who does not know anything about this project)
all he/she needs to know. The comments should usually include at least:
------------------------------------------------------------------------

PROJECT TITLE:              Physics - Particles 3

PURPOSE OF PROJECT:         To simulate physical interaction of particles with variable precision.
                            To model solid objects on a molecular level by using a single function representing 
                                the force between particles dependant on the distance between them

VERSION or DATE:            Fall 2015

HOW TO START THIS PROJECT:  Execute.main({});

from command line, the syntax is as follows:
java [-Xss108k] Execute [options]
Example: java Execute d0 z2 t512 sSandFall

Options: tag followed by value
    h - help
    l[file] - load
    v[file] - preview
    d# - debugging 
    z# - zoom 
    p# - precision 
    t# - max_threads 
    n# - simNum 
    s[str] - SIM

The block [-Xss108k] specifies the stack size of a thread.
If you use unlimited multithreading (mt_mode = 0), specify this 
    (the default is 1m (1mb))
debugging: 0: just a few messages 1:a few each frame 2: lots
max_threads: How much multithreading? 0:Unlimited   else:specify number

SIM: preset

AUTHORS:    Jonathan Black

USER INSTRUCTIONS:

    Toggle Pause with Spacebar

    Toggle record with 'r'

    Change Curser with:
        Up/Down Arrow: Cycle through curser shapes (Rectangle, Hexagon, Isometric Rectangle, Circle/ Annulus)
        Mouse Scroll: Change size
        Shift while Scrolling: Change only the width
        Control while Scrolling: Change only the height
        Hold both Shift and Control: height = width
        Right/Left Arrow: Change print density (Useful for making strong walls, but moving particles will freak out 
            when they are too close)
        Number Keys: Change Type (1: Sand, 2: Water, 3: Bomb, 4: Brick)
    
    Place Particles with mouse click
    Remove Particles with right mouse click (Only works properly with rectangular curser shape)
    
TO ADD:

    Zoom Window
    Time Resolution in frames per second (Based on gravity)
    Fix Removing with different curser shapes
    When zooming, make particle images bigger
# Creatures Sprites GIMP PlugIn 

Copyright (C) 2001  Tina Hirsch <tehirsch@nexgo.de>, updated 2008 Michael Maltese <mike@mikemaltese.com>

This plugin currently can load and save 
c16, s16 and blk images from the Creatures series.

Black (0,0,0) is converted to transparent like in the game
during loading and transparent in the image is converted 
to black when saving.

The c16 and s16 plugins handle the different images in one 
sprite via layers. The first image at the lowest layer
and the last on the top.

You can preview an animation by a rightclick in the image 
and choosing Filter->Animation->Play Animation.
Seperating the images from a sprite to single files and the
other way around is possible by rightclick and 
Video->Split Image to Frames respectively 
Video->Frames to Image. Please look for more information
about this in the GIMP User-manual.

### Linux

You need the libc16(-dev) ver. >=0.3 and gimp-dev packages in order 
to build and run this package.
To build and install the sourcepackage, just...

	./configure
	make
	make install

...and it's there.

### Windows

You need the libc16-dev package ver >=0.3, gimp-dev, gtk+-dev and glib-dev
packages in order to build (not run) this package. (The last three are
available from the Gimp for Windows homepage)
To build and install the sourcepackage, just...

	make -f Makefile.g95
	Copy the three exe's in src/ to GIMP's plug-ins directory

... and it's there too.


Enjoy

ofxAubio
========

[ofxAubio](https://aubio.org/ofxAubio) is an
[openFrameworks](http://openframeworks.cc) [addon](http://www.ofxaddons.com)
for [aubio](https://aubio.org).

Install
-------

### MacOSX

Fetch `ofxAubio` and `aubio.framework` from inside your openFrameworks root:

    $ cd /path/to/of_root/addons
    $ git clone git://git.aubio.org/git/ofxAubio/
    $ cd ofxAubio
    $ ./scripts/fetch_aubio_framework.sh

Select projectGenerator, select 'update project', then select the path of
`example_aubioDemo`, `/path/to/of_root/addons/ofxAubio/example_aubioDemo`.

Open `example_aubioDemo.xcodeproject`, drag `aubio.framework` into to it,
placing it in `frameworks / 3rd party frameworks`.

### Windows / Visual Studio 2015

Note: the included pre-compiled library files only work for x64, not x86. Binaries are available for x86 but I haven't added them. At this point I'm unsure if there are debug symbols included, but it successfully runs in both Debug & Release modes.

- Place `ofxAubio` in your openFrameworks addons folder.
- Use the projectGenerator to create or update a project, including ofxAubio as an addon
- The projectGenerator should set up the headers & .lib file properly for you
- Copy the `export/libaubio-4.dll` file into your bin folder so it sits next to your compiled application .exe

Project Homepage
----------------

The home page of ofxAubio can be found at: https://aubio.org/ofxAubio/

Copyright and License Information
---------------------------------

Copyright (C) 2003-2015 Paul Brossier <piem@aubio.org>

ofxAubio is free software: you can redistribute it and/or modify it under the
terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

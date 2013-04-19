## SimplicityNL (dutch)

![Action shot](https://raw.github.com/atkaper/pebble-simplicity-nl/master/releases/simplicity-nl.png)

Based on Simplicity & Complexity.


SimplicityNL is a quick mod of the Simplicity & Complexity watch face for Pebble which adds Week Day to the main screen.
It has been translated to Dutch, and items slightly repositioned / reformatted.
The text for date/weekday is only redrawn if changed to conserve juice.

Binary release:
https://github.com/atkaper/pebble-simplicity-nl/raw/master/releases/simplicity-nl.pbw


### Building the watch face

First, create a new project with the `create_pebble_project.py` script included in the [Pebble SDK](http://developer.getpebble.com).

    cd <parent dir of project root>

    /<sdk_path>/tools/create_pebble_project.py --symlink-only /<sdk_path>/sdk/ pebble-simplicity-nl
    cd pebble-simplicity-nl
    ./waf configure clean build

### Install the watch face using http server

This assumes you have build or downloaded the simplicity-nl.pbw on your machine, and have the SDK available.
Run:

    python -m SimpleHTTPServer 8000

Use your phone's web browser to browse to the pbw file in the build folder, and click it to install.



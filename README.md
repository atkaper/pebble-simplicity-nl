## SimpleWeek (dutch)

![Action shot](https://raw.github.com/atkaper/pebble-simpleweek-nl/master/releases/simpleweek.png)

Based on Simplicity & Complexity.


SimpleWeek is a quick and dirty mod of the Simplicity & Complexity watch face for Pebble which adds Week Day and Week Number to the main screen.
It has been translated to Dutch, and items slightly repositioned / reformatted.
The text for week/date/weekday is only redrawn if changed to conserve juice.

Binary release:
https://github.com/atkaper/pebble-simpleweek-nl/raw/master/releases/simpleweek.pbw


### Building the watch face

First, create a new project with the `create_pebble_project.py` script included in the [Pebble SDK](http://developer.getpebble.com).

    cd <parent dir of project root>

    /<sdk_path>/tools/create_pebble_project.py --symlink-only /<sdk_path>/sdk/ simpleweek

    cd simpleweek

    ./waf configure build

### Install the watch face using libpebble

First, make sure [libpebble](https://github.com/pebble/libpebble) is set up and running properly. Then:

    /<libpebble_path>/p.py --pebble_id <PEBBLE_ID_OR_MAC_ADDRESS> --lightblue load simpleweek.pbw


### Install the watch face using http server

Run:

    python -m SimpleHTTPServer 8000

Use your phone's web browser to browse to the pbw file in the build folder, and click it to install.



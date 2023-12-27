TA visual analytics
=====================

[![mbtaviz.github.io](http://mbtaviz.github.io/media/wide-preview-collage.png)](http://mbtaviz.github.io/)

vCore is a web based interactive visualization that
provides a glimpse into the performance and behavior of Trip Advisor.

## Quick Start

1. Install [node.js](http://nodejs.org/)
2. Setup command prompt in the path of the directory.
3. Serve up the website

    `http-server`

4. Browse to [http://localhost:8080/](http://localhost:8080/) to see the 
visualization

## Source Code Layout

    data\                post-processed visualization data
    scripts\             JavaScript files for the visualization and the website
    styles\              less CSS stylesheets and main.css that they are compiled into
    media\               Opengraph/Twitter Card images
    bower.json           bower dependencies
    favicon.ico          map glyph favicon with animation
    handout.pdf          design and implementation notes
    ie.png               website rendered to an image for browsers without svg support
    index.html           landing page
    README.md            README file that appears on the website's github page

## Regenerating Stylesheets

The visualization loads `style.css` which is generated from all of the less 
files in the `styles/` directory. If you change any of the less stylesheets 
use the less compile to regenerate `style.css` as described above:

## Raw Data

The raw data is available from two sources.  A compressed csv file with per-minute
turnstile entry and exit counts from each station is made available with 
permission from the MBTA:

<https://github.com/mbtaviz/mbtaviz.github.io/releases/download/data/turnstile_data.csv.gz>

NOTE: some stations don't accurately measure turnstile exits, so entry counts 
will tend to be more accurate.

Also the realtime subway and alert JSON files collected for the month of 
February are available here:

<https://github.com/mbtaviz/mbtaviz.github.io/releases/download/data/raw_subway_data.tar.gz>

They are stored in hourly gzipped files in the following format: 
`subway-line/yyyy/mm/dd/hh/data.json.gz`
where each line of the ungzipped file contains a JSON blob polled from the 
MBTA's realtime feed described
[here](http://www.mbta.com/rider_tools/developers/).  All times use Eastern 
Standard time zone.

## Creators

**Mike Barry**

- <https://github.com/msbarry>
- <https://twitter.com/msb5014>

**Brian Card**

- <https://github.com/bcard>
- <https://twitter.com/bmcard>

## License

Copyright 2014 Michael Barry and Brian Card.

JavaScript source files and less stylesheets released under the MIT License.

All other files including this README, the main web page, and images made available under
[Github's terms of service](https://help.github.com/articles/open-source-licensing)
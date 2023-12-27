TA visual analytics
=====================

[![mbtaviz.github.io](https://github.com/acies-sudharsan-shankar/Viz-Core/blob/main/media/Map.png)]()

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

Confidential.


TA visual analytics
=====================

[![mbtaviz.github.io](https://github.com/acies-sudharsan-shankar/Viz-Core/blob/main/media/Map.png)]()

vCore is a web based interactive visualization that
provides a glimpse into the performance and behavior of Trip Advisor.

## Quick Start

1. Install [node.js](http://nodejs.org/)
2. Setup command prompt in the path of the directory.
3. Install server

   `npm install http-server`
   `npm i -g serve`

4. Start the server

   `serve`

5. Serve up the website

    `http-server`

6. Browse to [http://localhost:8080/](http://localhost:8080/) to see the 
visualization

## Source Code Layout

    data\                post-processed visualization data
    scripts\             JavaScript files for the visualization and the website
    styles\              less CSS stylesheets and main.css that they are compiled into
    media\               Opengraph/Twitter Card images
    map.png              design and implementation notes
    index.html           landing page
    README.md            README file that appears on the website's github page

## Regenerating Stylesheets

The visualization loads `style.css` which is generated from all of the less 
files in the `styles/` directory. If you change any of the less stylesheets 
use the less compile to regenerate `style.css` as described above:


## Raw Data

Confidential.


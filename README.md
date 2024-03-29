# crypto-viz
A cryptocurrency visualization. Mostly used to practice using the wonderful d3.js and to appreciate the beauty of SVG. 


## Introduction
It's an exciting time for cryptocurrency. As of early March 2018, there are more than a thousand currencies in existence, with a combined [market capitalization](https://en.wikipedia.org/wiki/Market_capitalization) of roughly **USD $400 billion**.

For comparison, this is a little more than half the size of *Apple Inc.*, the largest publicly-traded company in the world, valued by markets according to its $375 billion in assets and $230 billion in annual revenues in 2017.

The aim of this visualization is to tell a story of the evolution of cryptocurrency. It shows the different directions the technology has gone, and which currencies have grown to be dominant in this emerging landscape.

Data for this visualization has been sourced from: [coinmarketcap.com](https://coinmarketcap.com/).

## Technology
This is a *Pie + Radar + Gauge Chart* written in JavaScript using **d3.js** and **SVG**.

This entire visualization is data driven. You can modify `data.csv` and the graphic will update accordingly. The one exception are the section labels which appear on each pie piece; these have been hand-positioned and are drawn from a static overlay file that you can find under `assets/`.

## Running

Just serve up the static files in this repository from a web server; then load it with a web browser.

For example:

```bash
$ npm install -g http-server
$ http-server .
# Open a browser to localhost:8080
```

It will take a little time to run, around 15 seconds on my current hardware. The visualization performs an exhaustive search when selecting a layout for the currencies. 

# Requirements
This visualization requires a somewhat modern browser to run. It uses some semi-recent JavaScript features, such as Maps, Sets, Generators and Arrow Functions.

It has been tested primarily in Chrome 64.0. It does render on Firefox 58.0, though text rendering seems to be incorrect (no support for `alignment-baseline`?).

# License and Attribution
This source code, and the official render of the visualization are dedicated to the public domain.
The data underlying this visualization is copyright [coinmarketcap.com](https://coinmarketcap.com/).


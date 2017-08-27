# kettlefish

![Kettlefish Logo](./src/lib/kettlefish.png)

# What is this

<<<<<<< HEAD
[Demo](http://htmlpreview.github.io/?https://github.com/paulbrzeski/kettlefish/blob/master/index.html)

# What is this

# Features

# Getting Started
=======
Kettlefish is a very simple boilerplate for fussy lazy web devs.

# Features
- Simple low maintenance configuration, works out of the box.
- [Pug](https://pugjs.org/) for HTML.
  - The [templates](/src/templates) folder contains page layouts, scripts blocks, etc and the [pages](/src/pages) folder creates the HTML structure of the site at the root, this is why there's a rogue index.html file in this repository. 
- [Stylus for CSS](http://stylus-lang.com/)
  - The [styles](/src/styles) folder compiles into CSS, as you'll note in the `css` script below, any files defined in `/src/styles` are compiled to CSS in `/dist`.
- [Rollup](https://rollupjs.org/) 
  - For ES2015, application development and compression.
- Example sites for even faster site building (coming soon)
  - For now, I've re-implemented the Semantic UI homepage demo using Kettlefish - [demo here](http://htmlpreview.github.io/?https://github.com/paulbrzeski/kettlefish/blob/master/index.html).

# How to use Kettlefish
If you're aware of some or all of the buzzwords in the features list, you're going to have a good time with this boilerplate. If not, feel free to post issues asking how to do things unrelated to this project.

Out of the box, you can start a new site using this as a base - you'll have everything you need to do anything. If you're a CMS developer, you can use this to implement a design first and then integrate it into your development pipeline.

## Scripts
Kettlefish comes with a couple of handy scripts out of the box. They are bound to package.json which you are welcome to use as a starting point for your own project.
```
  "scripts": {
    "build": "pug src/pages -P -o . -b . && stylus src/styles -o dist",
    "css": "stylus src/styles -o dist -w",
    "pug": "pug src/pages -P -o . -b . -w",
    "rollup": "rollup -c -w",
    "dev-osx": "sudo http-server -p 80 -c-1 .",
    "dev": "http-server -p 80 -c-1 .",
    "watch": "npm run css & npm run pug & npm run rollup & npm run dev",
    "gs": "for i in ../*; do (cd $i && (echo $i; git status)); done",
    "preinstall": "npm i -g http-server"
  }
```
>>>>>>> f19c0f105bc5a4749abbf0cd436085dc8d2429be

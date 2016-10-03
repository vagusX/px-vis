# px-slider [![Build Status](https://travis-ci.org/PredixDev/px-slider.svg?branch=master)](https://travis-ci.org/PredixDev/px-slider)

[![px-slider demo](px-slider.png?raw=true)](https://github.com/PredixDev/px-slider)

## Overview

The px-slider is a Predix UI component for defining a value in a range or a range of values within set boundaries.

## documentation

Read the full API and view the demo [here](https://predixdev.github.io/px-slider).

## Usage

### Prerequisites
1. node.js
2. npm
3. bower
4. [webcomponents-lite.js polyfill](https://github.com/webcomponents/webcomponentsjs)

Node, npm and bower are necessary to install the component and dependencies. webcomponents.js adds support for web components and custom elements to your application.

### Getting Started

First, install the component via bower on the command line.

```
bower install px-slider --save
```

Second, import the component to your application with the following tag in your head.

```
<link rel="import" href="/bower_components/px-slider/px-slider.html"/>
```

Finally, use the component in your application:

Single handled slider
```
<px-slider
  value="50"
  min="1"
  max="100">
</px-slider>
```

Multi-handled slider
```
<px-slider
  start-value="20"
  end-value="40"
  min="1"
  max="60">
</px-slider>
```

Single-handled slider with step
```
<px-slider
  value="250"
  step="50"
  min="0"
  max="500">
</px-slider>
```

### Layout

The slider will always take the full-width of whatever container it is in.
If resized or made visible for the first time (if the slider was in a modal for example) then the slider will need to be notified through the (iron-resizable-behavior)[https://elements.polymer-project.org/elements/iron-resizable-behavior?active=Polymer.IronResizableBehavior], by - for example - manually calling notifyResize() on it.


## Local Development

From the component's directory...

```
$ npm install
$ bower install
$ grunt sass
```

From the component's directory, to start a local server run:

```
$ grunt depserve
```

Navigate to the root of that server (e.g. http://localhost:8080/) in a browser to open the API documentation page, with link to the "Demo" / working examples.


### DevMode
Devmode runs `grunt depserve` and `grunt watch` concurrently so that when you make a change to your source files and save them, your preview will be updated in any browsers you have opened and turned on LiveReload.
From the component's directory run:

```
$ grunt devmode
```

### GE Coding Style Guide
[GE JS Developer's Guide](https://github.com/GeneralElectric/javascript)

<br />
<hr />

## Known Issues

Please use [Github Issues](https://github.com/PredixDev/px-slider/issues) to submit any bugs you might find.

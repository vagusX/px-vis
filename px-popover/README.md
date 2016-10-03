# Px-Popover [![Build Status](https://travis-ci.org/PredixDev/px-popover.svg?branch=master)](https://travis-ci.org/PredixDev/px-popover)

[![px-popover demo](px-popover.png?raw=true)](https://github.com/PredixDev/px-popover)


The px-popover is a Predix UI component for displaying additional information to a user.

## documentation

Read the full API and view the demo [here](https://predixdev.github.io/px-popover).

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
bower install px-popover --save
```

Second, import the component to your application with the following tag in your head.

```
<link rel="import" href="/bower_components/px-popover/px-popover.html"/>
```

Finally, use the component in your application:

Top popover
```
<div class="sample-container">
    <button id="btnUp" type="button" name="button">Up</button>
    <px-popover
        for="btnUp"
        orientation="top"
        popover-title="Top Popover"
        popover-body="Lorem ipsum dolor sit amet, consectetur elit, sed do eiusmod.">
    </px-popover>
</div>
```

Bottom popover
```
<div class="sample-container">
    <button id="btnUp" type="button" name="button">Bottom</button>
    <px-popover
        for="btnUp"
        orientation="bottom"
        popover-title="Bottom Popover"
        popover-body="Lorem ipsum dolor sit amet, consectetur elit, sed do eiusmod.">
    </px-popover>
</div>
```

Popover in a Relative position ancestor
```
<div class="sample-container" style="position:relative">
...
  <div style="position:relative>"
    <button id="btnRel" type="button" name="button">Bottom</button>
    <px-popover
        for="btnRel"
        orientation="bottom"
        popover-title="Bottom Popover"
        popover-body="Lorem ipsum dolor sit amet, consectetur elit, sed do eiusmod."
        position="relative" >
    </px-popover>
  </div>
  ...
</div>
```

### Layout

The popover has a fixed width but will grow vertically relative to its contents.

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
* Transformations on the target with position relative parent do not work. Instead, apply the transformation to the parent div so the popover gets it too.

Please use [Github Issues](https://github.com/PredixDev/px-popover/issues) to submit any bugs you might find.

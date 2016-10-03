px-overlay [![Build Status](https://travis-ci.org/PredixDev/px-overlay.svg?branch=master)](https://travis-ci.org/PredixDev/px-overlay)
-----------------------------------------------

[![px-overlay demo](px-overlay.png?raw=true)](https://predixdev.github.io/px-overlay)

## Overview

px-overlay is a Predix UI component that defines a full viewport overlay element. It has two types, a light version and a dark version.

## Usage

### Prerequisites
1. node.js
2. npm
3. bower
4. [webcomponents-lite.js polyfill](https://github.com/webcomponents/webcomponentsjs)

Node, npm and bower are necessary to install the component and dependencies. webcomponents.js adds support for web components and custom elements to your application.

## Getting Started

First, install the component via bower on the command line.

```
bower install px-overlay --save
```

Second, import the component to your application with the following tag in your head.

```
<link rel="import" href="/bower_components/px-overlay/px-overlay.html"/>
```

Finally, use the component in your application:

```
<px-overlay type="dark"></px-overlay>
```

<br />
<hr />
## documentation

Read the full API and view the demo [here](https://predixdev.github.io/px-overlay).
<br />
<hr />


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

### LiveReload

By default grunt watch is configured to enable LiveReload and will be watching for modifications in your root directory as well as `/css`.

Your browser will also need to have the LiveReload extension installed and enabled. For instructions on how to do this please refer to: [livereload.com/extensions/](http://livereload.com/extensions/).

Disable LiveReload by removing the `livereload` key from the configuration object or explicitly setting it to false.


### concurrent
concurrent runs `grunt depserve` and `grunt watch` concurrently so that when you make a change to your source files and save them, your preview will be updated in any browsers you have opened and turned on LiveReload.
From the component's directory run:

```
$ grunt concurrent
```

### GE Coding Style Guide
[GE JS Developer's Guide](https://github.com/GeneralElectric/javascript)

<br />
<hr />

## Known Issues

Please use [Github Issues](https://github.com/PredixDev/px-overlay/issues) to submit any bugs you might find.

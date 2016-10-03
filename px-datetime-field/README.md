#THIS COMPONENT IS NOT YET RELEASED.

Px-Datetime-field [![Build Status](https://travis-ci.org/PredixDev/px-datetime-field.svg?branch=master)](https://travis-ci.org/PredixDev/px-datetime-field)
-----------------------------------------------

[![px-datetime-field demo](px-datetime-field.png?raw=true)](https://github.com/PredixDev/px-datetime-field)

## Overview

Px-Datetime-field is a Predix Experience ('Px') component

## Getting Started

Read https://github.com/pages/PX/technical-principles/

From the component's directory...

```
$ npm install
$ bower install
$ grunt sass
```

### API and examples

https://predixdev.github.io/px-datetime-field/

### LiveReload

By default grunt depserve is configured to enable LiveReload and will be watching for modifications in your root directory as well as `/css`.

Your browser will also need to have the LiveReload extension installed and enabled. For instructions on how to do this please refer to [livereload.com/extensions/](http://livereload.com/extensions/).

Add, remove, modify file system patterns specified in the `depserve.options.livereload` array in your `Gruntfile.js`

This is an example depserve configuration:

```
depserve: {
    options: {
        open: '&lt;%= depserveOpenUrl %&gt;,
        livereload: [__dirname + "/js", __dirname + "/css", __dirname]
    }
}
```

Disable LiveReload by removing the `livereload` key from the configuration object.

### DevMode

From the component's directory run:

```
$ grunt devmode
```

Starts a local server exactly the same as if you had run `grunt depserve` however in addition it also runs `grunt watch` concurrently which will execute commands on file change according to the specified matching patterns.

This is an example `grunt watch` configuration which watches for changes to SASS files, then on changes executes SASS compilation and automatic prefixing:

```
watch: {
    sass: {
        files: ['sass/**/*.scss'],
        tasks: ['sass', 'autoprefixer'],
        options: {
            interrupt: true
        }
    }
}
```

### Options

Does this component have runtime configuration options?  If so, they should be able to be passed as attributes on the element with examples shown below.

### Function calls

What is the public API of this component?

### Extending styles

Documented CSS extension points?

### Extending behavior

See Polymer composition patterns

GE Coding Style Guide
---------------------

[GE JS Developer's Guide](https://github.com/GeneralElectric/javascript)


### Known Issues

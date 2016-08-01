px-overlay [![Build Status](https://travis-ci.org/PredixDev/px-overlay.svg?branch=master)](https://travis-ci.org/PredixDev/px-overlay)
-----------------------------------------------

[![px-overlay demo](px-overlay.png?raw=true)](https://github.com/PredixDev/px-overlay)

## Overview

px-overlay is a Predix UI component that defines a full viewport overlay element. It has two types, a light version and a dark version.

## Usage

```html

    <px-overlay type="dark"></px-overlay>

```
## documentation

Read the full API and view the demo [here](https://predixdev.github.io/px-overlay).

## Getting Started

Read https://github.com/pages/PX/technical-principles/

From the component's directory...

```
$ npm install
$ bower install
$ grunt sass
```

### API and examples

See the demo and read the full API <a href="https://predixdev.github.io/px-overlay">here</a>

```
$ grunt depserve
```

Starts a local server. Navigate to the root of that server (e.g. http://localhost:8080/) in a browser to open the API documentation page, with link to the "Demo" / working examples.

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

### Extending behavior

See Polymer [composition patterns](https://www.polymer-project.org/1.0/docs/devguide/behaviors.html)

### GE Coding Style Guide

[GE JS Developer's Guide](https://github.com/GeneralElectric/javascript)


### Known Issues
Please use [Github Issues](https://github.com/PredixDev/px-overlay/issues) to submit any bugs you might find.

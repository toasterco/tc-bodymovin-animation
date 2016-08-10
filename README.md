# tc-bodymovin-animation

`tc-bodymovin-animation` is used for creating a bodymovin animation. It deals with async loading of animation data and provides a loader when the animation is loading. Alternatively, it can be initialized with animation data passed directly to it.

All of the properties used to initialize Bodymovin have been exposed, however there are some methods that have not been exposed through the component. This is to avoid duplication of code. If a method exposed by Bodymovin, but not this component is needed, the bodymovin instance is exposed so it can be interacted with directly.

The Bodymovin API docs can be found here: [https://github.com/bodymovin/bodymovin](https://github.com/bodymovin/bodymovin)

Sample usage:

    <tc-bodymovin-animation 
        animation-json-url="../../bodymovin/demo/happy2016/data.json"
        autoplay
        loop></tc-bodymovin-animation>

To use animation data directly:

    <tc-bodymovin-animation 
        animation-data="[[animationData]]"
        autoplay
        loop></tc-bodymovin-animation>


### Styling

`<tc-bodymovin-animation>` provides the following custom properties and mixins for styling:

Custom property | Description | Default
----------------|-------------|----------
`--tc-bodymovin-animation-container` | Mixin applied to the bodymovin container. | `{}`
`--tc-bodymovin-animation-loader` | Mixin applied to the loader spinner | `{}`

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

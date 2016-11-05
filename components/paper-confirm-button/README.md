# \<paper-confirm-button\>

A button that asks for confirmation before performing an action

## Usage

Add the `<paper-confirm-button></paper-confirm-button>` to your page and add an action to be done once user confirms:
```html
<paper-confirm-button id="confirm">Action!</paper-confirm-button>
<script>
  let confirm = document.querySelector('#confirm'),
      action = ev => console.log('confirmed!');
  confirm.addEventListener('action-confirmed', action);
  confirm.addEventListener('action-canceled', ev => console.log('Canceled by user'));
</script>
```

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

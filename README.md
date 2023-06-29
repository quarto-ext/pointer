# pointer

A very simple RevealJS plugin extension that adds support for switching the cursor to a 'pointer' style element while presenting.

:warning: Requires Quarto Version 1.2.124 or later :warning:

## Installation

```
$ quarto add quarto-ext/pointer
```

This will install the extension under the `_extensions` subdirectory. If you're using version control, you will want to check in this directory.

## Usage

Simply add the extension to the list of reveal plugins like:

```
title: My Presentation
format:
    revealjs: default
    pointer:
      - # set pointer configuration options here
revealjs-plugins:
  - pointer
```

By default, you can activate the pointer mode by pressing the 'q' key while viewing the presentation. When activated, a 16px red pointer will be used as a cursor. Press the 'q' key once again to reactivate the standard cursor.

## Options

You can control the color and appearance of the pointer by passing some additional options under a `pointer` key. 

| Option | Description |
| --- | --- |
| ```key``` |  What key should be used to activate and deactivate the pointer. Defaults to `q`. |
| ```color``` | A CSS color name that provides the color used when the pointer is activated. Defaults to `red`. |
| ```pointerSize``` | The size of the pointer in pixels (please do not include units). Defaults to `16`. |
| ```alwaysVisible``` | Whether the pointer should always be visible, or disappear after it stops moving for a moment. Defaults to 'false'. |

## Example

View an example presentation at <https://quarto-ext.github.io/pointer/>. Use the 'q' to enable and disable the pointer.






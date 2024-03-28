# What is this?

These samples are JSON representations of DisplayLists from servo. The scope of the compositor is to take any list given in this format and render this on screen using the WebGPU API in Deno.

The samples here are created statically by running servo and capturing the print output from.
We use an old version in of our fork of servo: https://github.com/KnorpelSenf/servo/commit/61ad038d3b8dbaf919140739323914ffa49089b6

# Creating the DisplayLists Print Outputs

- clone our servo fork `git clone git@github.com:KnorpelSenf/servo.git`
- check it out `git checkout 61ad038d3b8dbaf919140739323914ffa49089b6`
- build it with `./mach build --dev`
- run it with the website, i.e. `./mach run tests/html/about-mozilla.html`
- The DisplayList is printed to the shell.

## Samples

Samples are in the format *Newline delimited JSON (NDJSON)*, see https://en.wikipedia.org/wiki/JSON_streaming

### 1. Local file [rect.html](./01-rect/rect.html)

Simple colored rectangle on colored background.

### 2. Local file hello.html [hello.html](./02-simple-text/hello.html)

Hello world! Copied from servo repository [hello.html](https://github.com/servo/servo/blob/66ad79501431cf0a5c83b15b7e443c87d780376e/tests/html/hello.html).

### 3. Local file [text-rendering.html](./03-text-rendering/text-rendering.html)

Different texts. Copied from servo repository [text_rendering.html](https://github.com/servo/servo/blob/66ad79501431cf0a5c83b15b7e443c87d780376e/tests/html/text_rendering.html).

### 4. Local file [about-mozilla.html](./04-about-mozilla/about-mozilla.html)

Copied from servo repository [about-mozilla.html](https://github.com/servo/servo/blob/66ad79501431cf0a5c83b15b7e443c87d780376e/tests/html/about-mozilla.html).

## Further reading

For a general overview how compositors work see https://wiki.mozilla.org/Gecko:Overview#Painting.2FRasterizing_.28Layers_aka_Non-WebRender.29

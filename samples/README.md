# What is this?

These samples are JSON representations of DisplayLists from servo. The scope of the compositor is to take any list given in this format and render this on screen using the WebGPU API in deno.

The samples here are created statically by running servo and capturing the print output from.
- We use an old version in the a fork of servo: https://github.com/KnorpelSenf/servo/commit/95aacd1b1d455f6100165d6ffebc228b2297d169
- check it out, build it with `./mach build --dev`
- run it with the the website, i.e. `./mach run tests/html/about-mozilla.html`

## Samples

Samples are in the format *Newline delimited JSON (NDJSON)*, see https://en.wikipedia.org/wiki/JSON_streaming

### 1. Local file about-mozilla.html

Copied from servo repository.

### 2. Local file hello.html

Hello world! Copied from servo repository.

### 3. Local file text-rendering.html

Different texts. Copied from servo repository.

### 4. Local file rect.html

Simple colored rectangle on colored background.


## Further reading
For a general overview how compositors work see https://wiki.mozilla.org/Gecko:Overview#Painting.2FRasterizing_.28Layers_aka_Non-WebRender.29
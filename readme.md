# Duplii Loading Spinner

This is the loading spinner we'll use when waiting for stuff to load asynchronously.

## Usage

All you need to do is enclose the form element or whatever you need to show a spinner for in a `.spinner-container` like this:

```html
<div class="spinner-container">
    <!-- stuff to be loaded -->
</div>
```

Please note that the content of the `.spinner-container` will be blurred and on top of that we will show the spinner. To start/stop the animation simply toggle the class `.spinning` to the container itself. Everything will fall into place.

I suggest you remove the focus from the element being clicked calling `blur()`. We are already preventing click events using `pointer-events: none;`, but that might not work on IE and does not remove the keyboard focus.

You might even go a step further and disable form elements altogether in order to prevent multiple submission.

## Live demo

A live demo of this project can be found [here](//duplii.github.io/duplii-loading-spinner "Duplii | Loading spinner animation").

![Loading spinner screenshot](http://duplii.github.io/duplii-loading-spinner/public/screenshot.png)

## MIT License

Copyright (c) 2015 Making Duplication Technologies ltd

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

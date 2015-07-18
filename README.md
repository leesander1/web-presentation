web-presentation
========

### A presentation framework created with web components

* Lightweight
* No dependencies
* Modular
* Extendable

## Example
http://christiankohler.github.io/web-presentation/


## Getting Started

Get web-presentation via bower

    bower install web-presentation

Include the `dist/web-presentation.html` file in your project.

    <link rel="import" href="web-presentation.html">

Use the web slide component in your html file.

```html
<web-presentation>
  <web-presentation-keyboardcontrols></web-presentation-keyboardcontrols>
  <web-slide-title>
    <h1>web-presentation</h1>
    <h2>Pure Webcomponents Presentation Framework</h2>
  </web-slide-title>
  <web-slide>
    <h1>Native, fast, extendable</h1>
    <h2>..and only one file to import</h2>
  </web-slide>
</web-presentation>
```

## API

### Components

|Component|Description|
|:--------|:----------|
|`web-presentation`|The presentation element which contains all slides|
|`web-slide`|The slide element has to be within a web-presentation element|
|`web-slide-title`|The title is the same element as web-slide. The idea is to make it easier to style all title slide|
|`web-presentation-keyboardcontrols`|One way to control the presentation. Use left and right arrow keys or space to go to the next slide|

### Transitions
Usage:

```html
  <web-slide-title data-transition="fall">
```

Available transitions:
* fall
* moveFromTop
* moveToLeft
* moveFromBottom

If you want to add a transitions to this library please make a pull-request.

## Run local demo
* Install local dev dependencies: `npm install`
* Run gulp `gulp`

## Requirements
Use Chrome 36 or higher to use web-presentation without a polyfill.

## Contribute
Help make web-presentation better.

* Install local dev dependencies: `npm install`
* Run gulp watch task: `gulp`
* Edit src files

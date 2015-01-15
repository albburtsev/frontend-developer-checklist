# Frontend-developer's checklist

## Usage

Open [source code of this file](https://raw.githubusercontent.com/albburtsev/frontend-developer-checklist/master/README.md) and copy next chapter into issue of your project. Enjoy!

## Checklist

### Common stuff: pages, styles, etc

- [ ] Adaptive design for typical resolutions
- [ ] [Viewport](https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag) meta tag
- [ ] Page 404
- [ ] Page 5xx
- [ ] Print version
- [ ] Noscript version
- [ ] Proper cache for all static files

### Graphics

- [ ] Favicon 16*16, 32*32
- [ ] Apple icons <sup>1</sup>
- [ ] Android icons <sup>2</sup>
- [ ] Support retina displays
- [ ] Sprites and icon fonts

### SEO and Social

- [ ] robots.txt
- [ ] humans.txt
- [ ] Social likes buttons
- [ ] [Facebook OG](https://developers.facebook.com/docs/opengraph/using-objects?locale=ru_RU#selfhosted-creating) meta tags
- [ ] [Twitter cards](https://dev.twitter.com/cards/markup) meta tags
- [ ] [GA](http://www.google.com/analytics/) and other statistic
- [ ] [Google webmasters](http://www.google.com/webmasters/)

### Validation and performance

 - [ ] [Google PageSpeed](https://developers.google.com/speed/pagespeed/) tools
 - [ ] [HTML validation](http://validator.w3.org/check)
 - [ ] [CSS validation](http://jigsaw.w3.org/css-validator/validator)
 - [ ] [Link checker](http://validator.w3.org/checklink)

### Build systems

 - [ ] Deploy task for build system
 - [ ] Default task for build system
 - [ ] Code style (jshint, jscs) for JavaScript code
 - [ ] Don't save builds in project's VCS
 - [ ] Check project's deployment (all stuff must be in config files: package.json, bower.json)
 - [ ] ```npm test``` required

## Footnotes

<sup>[1] Apple icons</sup>

```html
<link rel="apple-touch-icon" href="57x57.png">
<link rel="apple-touch-icon" href="72x72.png" sizes="72x72">
<link rel="apple-touch-icon" href="114x114.png" sizes="114x114">
<link rel="apple-touch-startup-image" href="57x57.png">
```

<sup>[2] Android icons</sup>

```html
<link rel="icon" sizes="192x192" href="nice-highres.png">
<link rel="icon" sizes="128x128" href="niceicon.png">
```
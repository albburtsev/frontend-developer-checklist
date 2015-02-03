# Frontend-developer's checklist

## Usage

Open [source code of this file](https://raw.githubusercontent.com/albburtsev/frontend-developer-checklist/master/README.md) and copy next chapter into issue of your project. Enjoy!

## Checklist

### Common stuff: pages, styles, etc

- [ ] Check responsive design for typical resolutions (320, 480, 1024, 1600, 2k)
- [ ] [Viewport](https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag) meta tag
- [ ] X-UA-Compatible meta tag <sup>1</sup>
- [ ] Format detection meta tags <sup>2</sup>
- [ ] Page 404
- [ ] Page 5xx
- [ ] Print version
- [ ] Noscript version
- [ ] Proper cache for all static files
- [ ] [Apple-specific](https://developer.apple.com/library/safari/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/MetaTags.html) meta tags
- [ ] All absolute pathes without protocol

### Graphics

- [ ] Favicon 16x16, 32x32 <sup>3</sup>
- [ ] Apple icons <sup>4</sup>
- [ ] Android icons <sup>5</sup>
- [ ] Support retina displays
- [ ] Sprites and icon fonts
- [ ] Minify all images with [Imagemin](https://github.com/gruntjs/grunt-contrib-imagemin)
- [ ] Image inlining (for instance [in Stylus](http://learnboost.github.io/stylus/docs/functions.url.html))

### SEO and Social

- [ ] robots.txt
- [ ] humans.txt
- [ ] Mark up content with [microdata](http://schema.org/)
- [ ] Social likes buttons
- [ ] Common meta tags <sup>6</sup>
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
 - [ ] Code style (jshint, jscs) for JavaScript code
 - [ ] [Autoprefixer](https://github.com/postcss/autoprefixer) for all styles
 - [ ] Don't save builds in project's VCS
 - [ ] Check project's deployment (all stuff must be in config files: package.json, bower.json)
 - [ ] ```npm test``` required

---------------------------------------

<sup>[1] X-UA-Compatible</sup>

```html
<meta http-equiv="X-UA-Compatible" content="IE=edge">
```

<sup>[2] Format detection</sup>

```html
<meta name="format-detection" content="telephone=no"/>
<meta name="format-detection" content="address=no"/>
```

<sup>[3] Favicon</sup>

```html
<link rel="shortcut icon" type="image/x-icon" href="path/to/icon.ico"/>
```

<sup>[4] Apple icons</sup>

```html
<link rel="apple-touch-icon" href="57x57.png">
<link rel="apple-touch-icon" href="72x72.png" sizes="72x72">
<link rel="apple-touch-icon" href="114x114.png" sizes="114x114">
<link rel="apple-touch-startup-image" href="57x57.png">
```

<sup>[5] Android icons</sup>

```html
<link rel="icon" sizes="192x192" href="nice-highres.png">
<link rel="icon" sizes="128x128" href="niceicon.png">
```

<sup>[6] Common meta tags</sup>

```html
<meta name="description" content="" />
<meta name="keywords" content="" />
<meta name="author" content="" />
<meta name="copyright" content="" /> 
```

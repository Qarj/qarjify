# moshified.com - HTML and CSS course

## Extensions

-   HTML CSS Support 1.3.3
-   CSS Peek 4.0.2
-   Prettier
-   Highlight Matching Tag
-   ToDo Highlight 1.0.4
-   Live Server 5.6.1

## Setup

Create `index.html` then type `!` and press tab to get a basic html template.

## Identifying the Components

-   Moshify logo
-   Navigation bar
-   Hero component

    -   Banner with title and subtitle
    -   Get started button
    -   Graphic

-   Input field with button inside
-   inline list
-   multiple instances of the badge component
-   cards
    -   badge component
    -   list with green ticks
-   icons
-   links
-   two column grid component
-   media components / media object
-   quotes / testimonials
-   callout component
-   footer

## Colour Palette

-   Primary: dark blue
-   Secondary: light blue
-   Accent: red

## Emmet

-   `ul>li*5` - unordered list with 5 list items
-   `ul.list>li{item $}*3` - unordered list with class list and 3 list items

## The Open Graph protocol

Created by Facebook to allow the website to control how content is displayed when a link is shared on social media.

Checkout the [Open Graph protocol](https://ogp.me/) for more information.

## HTML Validator

https://validator.w3.org/nu/#textarea

## CSS Validator

https://jigsaw.w3.org/css-validator/#validate_by_input

## Building for Production

-   Combine CSS and JS files
-   Minify CSS and JS files
-   Compress images

Webpack is the most popular. Requires a lot of configuration.
Rollup is a simpler alternative.
Parcel is a zero configuration bundler.

Install Parcel.

```sh
npm install --save-dev parcel-bundler
```

### One way to launch

```sh
node_modules/.bin/parcel index.html
```

### Install globally

```sh
npm install -g parcel-bundler
```

### Launch

```sh
parcel index.html
```

### Build for production

Delete the dist folder first to otherwise there might be dev files in the dist folder.

```sh
parcel build index.html
.
/home/tim/git/scrapbook/html5/moshified/index.html: tree.render is not a function
```

Turn off ninify of SVG files to prevent the build error.

Add `.htmlnanorc` file to the project root.

```json
{
    "minifySvg": false
}
```

## Deployment with Netlify

Link GitHub repo to Netlify.

Set the build command to `parcel build index.html`.

Set the publish directory to `dist`.

Click `Deploy site`.

Change the site name to https://qarjified.netlify.app

## Measure performance

https://web.dev/measure/

## Normalize.css

```css
@import "./normalize.css";
```

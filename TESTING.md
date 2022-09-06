# Testing

# Bugs and Fixes

- When testing on different browsers, the portfolio page grid looked streched on Safari and some iPhones. Searching google, I found that this is a common problem with how the browser reads heights in the Grid. The solution was found [here](https://newbedev.com/why-is-css-grid-row-height-different-in-safari) which fixed the issue.
[Safari issue](/docs/safariportfolio1.png)

# Lighthouse Testing

## index.html

### Desktop
- The index page required accessibilty controls for ARIA - these have all been added.
- Scroll to top #top needed hidden on css and aria controls.
- The images are recommended to be in a next-gen format to speed loading, I have changed these images to webp with mentor Kera Cudmore's advice using www.birme.net and the advice found [here](https://www.stefanjudis.com/snippets/a-picture-element-to-load-correctly-resized-webp-images-in-html/)
The images have a back up for incompatible browsers.
````
        <picture>
          <source srcset="assets/images/conan-evidence-of-immortality.webp"     alt="conan-evidence of immortality cover" class="image" type="image/webp">
          <img src="assets/images/conan-evidence-of-immortality.jpg"    alt="conan-evidence of immortality cover" class="image" type="image/jpg">
        </picture>
````
- Image elements do not have explicit width and height - fixed with this code from https://web.dev/optimize-cls/?utm_source=lighthouse&utm_medium=devtools#images-without-dimensions

````
img {
  aspect-ratio: attr(width) / attr(height);
}
````

### Mobile

## portfolio.html

### Desktop
- The page required accessibilty controls for ARIA - these have all been added.
- Scroll to top #top needed hidden on css and aria controls.
- The main image was also recommended to be changed to a next-gen format to speed loading, I have changed these images to webp with mentor Kera Cudmore's advice using www.birme.net and the advice found [here](https://www.stefanjudis.com/snippets/a-picture-element-to-load-correctly-resized-webp-images-in-html/)
The images have a back up for incompatible browsers.



### Mobile




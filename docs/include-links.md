# About Page Link Fixes

## item-figure link
- Go to `_includes/feature/item-figure.html`
- In the html code, find the anchor element (`<a>`). It will look like this: `<a href="{{ '/item.html' | relative_url | append: '?id=' | append: item.objectid }}">`
- Change `append: item.objectid` to `append: figure.objectid`
- Commit your changes

## item-pdf-embed link
- Go to `_includes/feature/item-pdf-embed.html`
- In the html code, locate the anchor element `<a>` inside the `<figure>` element. It will look like this: `<a href="{{ '/items/' | append: item.objectid | append: '.html' | relative_url }}">`
- Replace this content with the following line of code: `<a href="{{ '/item.html' | relative_url | append: '?id=' | append: item.objectid }}">`
- Commit your changes
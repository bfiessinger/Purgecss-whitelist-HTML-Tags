# Purgecss HTML Tags Whitelist
purgecss whitelist for all available HTML Tags.

## Getting started
First install [purgecss](https://github.com/FullHuman/purgecss).

## Installation
`npm i --save-dev purgecss-whitelist-htmltags`

## Usage
```javascript
const purgecssHTMLTags = require('purgecss-whitelist-htmltags');

module.exports = {
	...
	plugins: [
    new PurgecssPlugin({
      paths: PurgecssFiles,
      whitelist: [
        ...
				purgecssHTMLTags.whitelist,
				...
      ]
    })
	],
	...
}
```

# Purgecss HTML Tags Whitelist
purgecss whitelist for all available HTML Tags.

## Getting started
First install [purgecss](https://github.com/FullHuman/purgecss).

## Installation
`npm i --save-dev purgecss-whitelist-htmltags`

## Usage
```javascript
import Purgecss from 'purgecss';
import purgecssWithHtml from 'purgecss-whitelist-htmltags';

const purgeCss = new Purgecss({
	whitelist: purgecssWithHtml.whitelist,
	whitelistPatterns: purgecssWithHtml.whitelistPatterns
});

const res = purgeCss.purge();
```

if you have additional classes for whitelist or whitelistPattners, you can use the spread operator:

```javascript
whitelist: [
	...purgecssWithHtml.whitelist,
	...thirdparty.whitelist,
	'my-class'
],
whitelistPatterns: [
	...purgecssWithHtml.whitelistPatterns,
	...thirdparty.whitelistPatterns,
	/^my-(class|id)$/
]
```

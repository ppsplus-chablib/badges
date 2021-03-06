<!-- TITLE/ -->

<h1>badges</h1>

<!-- /TITLE -->


<!-- BADGES/ -->

<span class="badge-travisci"><a href="http://travis-ci.org/bevry/badges" title="Check this project's build status on TravisCI"><img src="https://img.shields.io/travis/bevry/badges/master.svg" alt="Travis CI Build Status" /></a></span>
<span class="badge-npmversion"><a href="https://npmjs.org/package/badges" title="View this project on NPM"><img src="https://img.shields.io/npm/v/badges.svg" alt="NPM version" /></a></span>
<span class="badge-npmdownloads"><a href="https://npmjs.org/package/badges" title="View this project on NPM"><img src="https://img.shields.io/npm/dm/badges.svg" alt="NPM downloads" /></a></span>
<span class="badge-daviddm"><a href="https://david-dm.org/bevry/badges" title="View the status of this project's dependencies on DavidDM"><img src="https://img.shields.io/david/bevry/badges.svg" alt="Dependency Status" /></a></span>
<span class="badge-daviddmdev"><a href="https://david-dm.org/bevry/badges#info=devDependencies" title="View the status of this project's development dependencies on DavidDM"><img src="https://img.shields.io/david/dev/bevry/badges.svg" alt="Dev Dependency Status" /></a></span>
<br class="badge-separator" />
<span class="badge-patreon"><a href="https://patreon.com/bevry" title="Donate to this project using Patreon"><img src="https://img.shields.io/badge/patreon-donate-yellow.svg" alt="Patreon donate button" /></a></span>
<span class="badge-flattr"><a href="https://flattr.com/profile/balupton" title="Donate to this project using Flattr"><img src="https://img.shields.io/badge/flattr-donate-yellow.svg" alt="Flattr donate button" /></a></span>
<span class="badge-liberapay"><a href="https://liberapay.com/bevry" title="Donate to this project using Liberapay"><img src="https://img.shields.io/badge/liberapay-donate-yellow.svg" alt="Liberapay donate button" /></a></span>
<span class="badge-thanksapp"><a href="https://givethanks.app/donate/npm/badges" title="Donate to this project using Thanks App"><img src="https://img.shields.io/badge/thanksapp-donate-yellow.svg" alt="Thanks App donate button" /></a></span>
<span class="badge-boostlab"><a href="https://boost-lab.app/bevry/badges" title="Donate to this project using Boost Lab"><img src="https://img.shields.io/badge/boostlab-donate-yellow.svg" alt="Boost Lab donate button" /></a></span>
<span class="badge-buymeacoffee"><a href="https://buymeacoffee.com/balupton" title="Donate to this project using Buy Me A Coffee"><img src="https://img.shields.io/badge/buy%20me%20a%20coffee-donate-yellow.svg" alt="Buy Me A Coffee donate button" /></a></span>
<span class="badge-opencollective"><a href="https://opencollective.com/bevry" title="Donate to this project using Open Collective"><img src="https://img.shields.io/badge/open%20collective-donate-yellow.svg" alt="Open Collective donate button" /></a></span>
<span class="badge-crypto"><a href="https://bevry.me/crypto" title="Donate to this project using Cryptocurrency"><img src="https://img.shields.io/badge/crypto-donate-yellow.svg" alt="crypto donate button" /></a></span>
<span class="badge-paypal"><a href="https://bevry.me/paypal" title="Donate to this project using Paypal"><img src="https://img.shields.io/badge/paypal-donate-yellow.svg" alt="PayPal donate button" /></a></span>
<span class="badge-wishlist"><a href="https://bevry.me/wishlist" title="Buy an item on our wishlist for us"><img src="https://img.shields.io/badge/wishlist-donate-yellow.svg" alt="Wishlist browse button" /></a></span>

<!-- /BADGES -->


<!-- DESCRIPTION/ -->

The definitive collection of badges for rendering

<!-- /DESCRIPTION -->


<!-- INSTALL/ -->

<h2>Install</h2>

<a href="https://npmjs.com" title="npm is a package manager for javascript"><h3>npm</h3></a>
<ul>
<li>Install: <code>npm install --save cb-badges</code></li>
<li>Require: <code>require('cb-badges')</code></li>
</ul>

<a href="https://jspm.io" title="Native ES Modules CDN"><h3>jspm</h3></a>

``` html
<script type="module">
    import * as pkg from '//dev.jspm.io/cb-badges'
</script>
```

This project provides its type information via inline <a href="http://usejsdoc.org" title="JSDoc is an API documentation generator for JavaScript, similar to Javadoc or phpDocumentor">JSDoc Comments</a>. To make use of this in <a href="https://www.typescriptlang.org/" title="TypeScript is a typed superset of JavaScript that compiles to plain JavaScript. ">TypeScript</a>, set your <code>maxNodeModuleJsDepth</code> compiler option to `5` or thereabouts. You can accomlish this via your `tsconfig.json` file like so:

``` json
{
  "compilerOptions": {
    "maxNodeModuleJsDepth": 5
  }
}
```

<!-- /INSTALL -->


## Usage

``` javascript
// Listing of badges to output
const list = [
  // Custom Badges
  ['badge', {image: 'image', alt: 'alt'}],
  ['badge', {image: 'image', alt: 'alt', url: 'url', title: 'title'}],
  ['shields', {left: 'left', right: 'right', alt: 'alt', url: 'url', title: 'title'}],
  ['shields', {left: 'left', right: 'right', color: 'red', alt: 'alt', url: 'url', title: 'title'}]
]

// Configuration for the badges
const config = {
}

// Options for rendering the badges
const options = {
	// Filter Category
	// When set to a string, will only render badges from the list that of the specified category
	// Values can be 'development', 'testing', 'funding', or 'social'
	// E.g. to render only funding badges, set to 'funding'
	filterCategory: false,

	// Filter Scripts
	// When true, do not render any badges from the list that are scripts
	filterScripts: false
}

// Render the badges to a string
const result = require('cb-badges').renderBadges(list, config, options)

// Output the result
console.log(result)
```

<!-- BACKERS/ -->

<h2>Backers</h2>

<h3>Maintainers</h3>

These amazing people are maintaining this project:

<ul><li><a href="http://balupton.com">Benjamin Lupton</a> — <a href="https://github.com/bevry/badges/commits?author=balupton" title="View the GitHub contributions of Benjamin Lupton on repository bevry/badges">view contributions</a></li></ul>

<h3>Sponsors</h3>

<h3>Contributors</h3>

These amazing people have contributed code to this project:

<ul><li><a href="http://balupton.com">Benjamin Lupton</a> — <a href="https://github.com/bevry/badges/commits?author=balupton" title="View the GitHub contributions of Benjamin Lupton on repository bevry/badges">view contributions</a></li>
<li><a href="https://github.com/digitalsadhu">Richard Walker</a> — <a href="https://github.com/bevry/badges/commits?author=digitalsadhu" title="View the GitHub contributions of Richard Walker on repository bevry/badges">view contributions</a></li></ul>

<!-- /BACKERS -->


<!-- LICENSE/ -->

<h2>License</h2>

<ul><li><a href="http://spdx.org/licenses/MIT.html">MIT License</a></li></ul>

<!-- /LICENSE -->

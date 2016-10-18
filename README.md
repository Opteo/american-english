# american-english
Easily check American / English spelling differences

### Installation
```bash
$ npm install american-english
```

### Example
```javascript
const spelling = require('american-english')

const uk_word = 'colour'
let uk_word_to_american = spelling.toUS(uk_word)

const us_word = 'color'
let us_word_to_english = spelling.toUK(us_word)

if(spelling.hasUSDifference('colour')) {
	// Difference between 'colour' found
	console.log(spelling.toUS('colour'))
}

if(spelling.hasUKDifference('color')) {
	// Difference between 'color' found
	console.log(spelling.toUK('color'))
}
```
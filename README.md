# american-english
Easily check American / English spelling differences

### Installation
```bash
$ npm install american-english
```

### Usage
```javascript
const spelling = require('american-english')

const uk_word = 'colour'
let uk_word_to_american = spelling.toUS(uk_word) // 'color'

const us_word = 'color'
let us_word_to_english = spelling.toUK(us_word) // 'colour'

if(spelling.hasUSDifference('colour')) {
	// Difference between 'colour' found
	console.log(spelling.toUS('colour'))
}

if(spelling.hasUKDifference('color')) {
	// Difference between 'color' found
	console.log(spelling.toUK('color'))
}
```

### Spellings
List obtained from [http://www.tysto.com/uk-us-spelling-list.html](http://www.tysto.com/uk-us-spelling-list.html). Feel free to make a pull request if a spelling difference is not found correctly with this package.
parse-whois
=========

Parses WhoIs lookup data from a text string to an Array of JSON object

## Installation

```shell
	npm install parse-whois --save
```

## Usage

data is the raw out

```js
	var parser = require('parse-whois');
	var whois = require('node-whois');

	whois.lookup('github.com', function(err, data){
		if (err) throw err;

		console.log(data);

		console.log(parser.parseWhoIsData(data));
	});

```

## Test

```js
	npm test
```

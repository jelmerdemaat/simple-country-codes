# Simple country codes
[GitHub](https://github.com/jelmerdemaat/simple-country-codes) | [NPM](https://www.npmjs.com/package/simple-country-codes) | [@jelmerdemaat](https://twitter.com/jelmerdemaat)

Retrieve country names by giving country codes.

All this is:
- A JSON object of all country codes and their country names
- A function to safely retrieve items from that object

Features:
* ES6 ready
* Case insensitive ('gb' and 'GB' both work)
* Function `getCountry` checks existance of property with `object.hasOwnProperty`
* Returns `false` if your query does not exist

## Usage

Add to your local dependencies using [npm](https://docs.npmjs.com/getting-started/installing-npm-packages-locally):

```bash
npm install --save simple-country-codes
```

[Import](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import) and use in your own JavaScript:

```js
import { getCountry } from 'simple-country-codes';

getCountry('gb'); // Returns "United Kingdom"
getCountry('nl'); // Returns "Netherlands"
getCountry('poop'); // Returns false
```

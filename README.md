<p align="center">
  <img src="/src/assets/pluraljs.svg" />
</p>
<h3 align="center">
  PluralJS
</h3>

<p align="center">
  <a href="https://npmjs.org/package/pluraljs" target="_blank" rel="noopener">
    <img src="https://img.shields.io/npm/v/pluraljs.svg?style=flat" alt="npm version">
  </a>
    <img src="https://img.shields.io/github/size/kalpeshsingh/pluraljs/src/main.js.svg?style=flat" alt="File size">
     <a href="https://npmjs.org/package/pluraljs" target="_blank" rel="noopener">
        <img src="https://img.shields.io/npm/dm/pluraljs.svg?style=flat" alt="npm downloads">
     </a>
</p>

<p  align="center">A micro library to produce any singular noun into plural
  
### 💡 Motive
---
I was curious to learn about how to build a library, what are the thought-processes behind it, what are the technical stuff you need to know etc. This was the primary reason PluralJS came into conception.

### 📥 Installation

---

**via npm**

```shell
npm install pluraljs --save
```

**via yarn**

```shell
yarn add pluraljs
```

**via CDN direct link**

```html
<script src="https://cdn.jsdelivr.net/npm/pluraljs/dist/pluraljs.umd.min.js"></script>
<!-- or -->
<script src="https://unpkg.com/pluraljs/dist/pluraljs.umd.min.js"></script>
```

**direct download**

```shell
curl -o https://unpkg.com/pluraljs/dist/pluraljs.umd.min.js
```

### 📑 Usage

---

The PluralJS is single responsibility library.
It takes only a noun (with optional count parameter) and produce plural noun out of it.

#### API

| parameter | description                       | type   | required | example                                                    |
| --------- | --------------------------------- | ------ | -------- | ---------------------------------------------------------- |
| word      | a word to pluralize               | string | yes      | pluralJs('cat') // cats                                    |
| count     | pluralize the word based on count | number | no       | pluralJs('cat', 3) // cats <br/> pluralJs('cat', 1) // cat |

#### Node

```node
const pluralJs = require('pluraljs');
console.log(pluralJs('cat')); // cats

console.log(pluralJs('cat', 1)); // cat
console.log(pluralJs('cat', 3)); // cats
```

#### ES6

```js
import pluraJs from 'pluraljs';
console.log(pluralJs('cat')); // cats

console.log(pluralJs('cat', -4)); // cat
```

#### Browser

```html
<script src="https://cdn.jsdelivr.net/npm/pluraljs/dist/pluraljs.umd.min.js"></script>
<script>
	console.log(pluralJs('cat')); // cats
	console.log(pluralJs('cat', '4')); // cats
</script>
```

### 🧡 Show little more care in your product

---

| Product without words pluralization                                                                                  | Product using PluralJS                                                                                        |
| -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| <img width="300px" src="/src/assets/sample_without_pluralization.png" alt="Screenshot - Product not using PluralJS"> | <img width="300px" src="/src/assets/sample_with_pluralization.png" alt="Screenshot - Product using PluralJS"> |

### 📋 Changelog

---

**1.1.0**

- `ENHANCEMENT` Added ability to pass count parameter

**1.0.0**

- `FEATURE` Released first stable version

### 💂‍♂️Maintainer

---

Kalpesh Singh ([@knowkalpesh](https://twitter.com/knowkalpesh))

### 🙇 Credits

---

- The core logic and testing file are borrowed from [Blake Embrey](https://github.com/blakeembrey)'s [Pluralize](https://github.com/blakeembrey/pluralize)
- Card screenshot used from [Chakra UI](https://chakra-ui.com/)
- Those lovely cats artwork used for branding is from [Undraw](https://undraw.co/)

### ⚖️ License

---

kalpeshsingh/PluralJS is licensed under the [MIT license](https://opensource.org/licenses/MIT).

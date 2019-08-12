# `@elunic/ecs`

[![Build Status](https://travis-ci.org/elunic/ecs.svg?branch=master)](https://travis-ci.org/elunic/ecs)

The elunic coding styles

## Table of Contents

- [`@elunic/ecs`](#elunicecs)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
    - [`tsconfig`](#tsconfig)
    - [`tslint`](#tslint)
      - [`tslint-react` `peerDependency` for React](#tslint-react-peerdependency-for-react)
    - [Prettier](#prettier)
    - [EditorConfig](#editorconfig)
    - [`commitlint`](#commitlint)
  - [License](#license)

## Installation

```bash
$ npm install @elunic/ecs
```


## Usage

### `tsconfig`

* `tsconfig/tsconfig.json`
* `tsconfig/tsconfig.prod.json`

Example usage for your `/tsconfig.json`:
```json
{
  "extends": "@elunic/ecs/tsconfig/tsconfig.json",
  "rules": {
  }
}
```

### `tslint`

* `tslint/tslint.json`
* `tslint/tslint.fix.json`
* `tslint/tslint-angular7.json`
* `tslint/tslint-angular7.fix.json`
* `tslint/tslint-angular8.json`
* `tslint/tslint-angular8.fix.json`
* `tslint/tslint-react16.json`
* `tslint/tslint-react16.fix.json`

Example usage for your `/tslint.json`:
```json
{
  "extends": "@elunic/ecs/tslint/tslint.json",
  "rules": {
  }
}
```

#### `tslint-react` `peerDependency` for React

For React, the `tslint-react` `peerDependency` is required. 

### Prettier

* `prettier/prettier.config.js`

Example usage for your `/prettier.config.js`:
```javascript
module.exports = require('@elunic/ecs/prettier');
```

### EditorConfig

* `editorconfig/.editorconfig`

Must currently be included by copying it to your project root.

### EditorConfig

* `commitlint/index.js`

Must currently be included by copying it to your project root.

Example usage for your `/commitlint.config.js`:
```javascript
module.exports = {
	extends: ['@elunic/ecs/commitlint'],
};
```


## License

MIT License

Copyright (c) 2019 elunic AG/William Hefter <wh@elunic.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

# `@elunic/ecs`

[![Build Status](https://travis-ci.org/elunic/ecs.svg?branch=master)](https://travis-ci.org/elunic/ecs)

The elunic coding styles

## Table of Contents

- [`@elunic/ecs`](#elunicecs)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
    - [`tsconfig`](#tsconfig)
    - [`eslint`](#eslint)
    - [`tslint`](#tslint)
      - [`tslint-react` `peerDependency` for React](#tslint-react-peerdependency-for-react)
    - [Prettier](#prettier)
    - [EditorConfig](#editorconfig)
    - [Commitlint](#commitlint)
  - [License](#license)

## Installation

```bash
$ npm install @elunic/ecs
```

## Usage

### `tsconfig`

- `tsconfig/tsconfig.json`
- `tsconfig/tsconfig.prod.json`

Example usage for your `/tsconfig.json`:

```json
{
  "extends": "@elunic/ecs/tsconfig/tsconfig.json",
  "rules": {}
}
```

### `eslint`

There is currently no `eslint` configuration for Angular, as Angular itself
has not yet switched to using `eslint`. For Angular projects, `tslint` should still be used.

- `eslint/.eslintrc.json`
- `eslint/.eslintrc.fix.json`

Example usage for your `/.eslintrc.json`:

```json
{
  "extends": "@elunic/ecs/eslint/.eslintrc.json",
  "rules": {}
}
```

### `tslint`

Note that `tslint` is deprecated with an expected EOL at the end of 2020.

Currently, the `tslint` configurations for **Angular** are still in use because Angular has
not yet switched to `eslint`.

- `tslint/tslint.json`
- `tslint/tslint.fix.json`
- `tslint/tslint-angular7.json`
- `tslint/tslint-angular7.fix.json`
- `tslint/tslint-angular8.json`
- `tslint/tslint-angular8.fix.json`
- `tslint/tslint-react16.json`
- `tslint/tslint-react16.fix.json`

Example usage for your `/tslint.json`:

```json
{
  "extends": "@elunic/ecs/tslint/tslint.json",
  "rules": {}
}
```

#### `tslint-react` `peerDependency` for React

For React, the `tslint-react` `peerDependency` is required.

### Prettier

- `prettier/prettier.config.js`

Example usage for your `/.prettierrc.json`:

```javascript
"@elunic/ecs/prettier"
```

### EditorConfig

- `editorconfig/.editorconfig`

Must currently be included by copying it to your project root.

### Commitlint

- `commitlint/index.js`

Example usage for your `/.commitlintrc.json`:

```javascript
{
  "extends": [
    "@elunic/ecs/commitlint"
  ]
}
```

## License

MIT License

Copyright (c) 2019-2020 elunic AG/William Hefter <wh@elunic.com>

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

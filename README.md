# eslint-plugin-no-only-tests

[![Version](https://img.shields.io/npm/v/eslint-plugin-no-only-tests.svg)](https://www.npmjs.com/package/eslint-plugin-no-only-tests) [![CircleCI](https://circleci.com/gh/levibuzolic/eslint-plugin-no-only-tests.svg?style=shield)](https://circleci.com/gh/levibuzolic/eslint-plugin-no-only-tests)

ESLint rule for `(describe|it|context|tape|test).only` in [mocha](https://mochajs.org/) and other JS library tests.

## Installation

First you'll need to install [ESLint](http://eslint.org) and the plugin:

```
npm install --save-dev eslint eslint-plugin-no-only-tests
# OR
yarn add --dev eslint eslint-plugin-no-only-tests
```

**Note:** If you installed ESLint globally (using the `-g` flag) then you must also install `eslint-plugin-no-only-tests` globally.

## Usage

Add `no-only-tests` to the plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
  "plugins": [
    "no-only-tests"
  ]
}
```

Then configure the rules you want to use under the rules section.

```json
{
  "rules": {
    "no-only-tests/no-only-tests": 2
  }
}
```


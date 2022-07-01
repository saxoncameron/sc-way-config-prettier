> `@sc-way`: The *way* SC (@saxoncameron) likes to do things.

# Prettier config

An importable, installable [Prettier](https://prettier.io/) config based on the author's personal preferences.

ℹ️ Note: this includes an [`.editorconfig`](https://editorconfig.org/) under the hood as well.

## Install

1. First install the config package:

```sh
#npm
npm install --save-dev @sc-way/config-prettier

#yarn
yarn --dev @sc-way/config-prettier

```

2. and then reference it, in one of the following ways:
- in `package.json`:
	- Add this line: `"prettier": "@sc-way/config-prettier"`
- or if you prefer to keep it in a separate config file: `.prettierrc.js`
	- `module.exports = require("@sc-way/config-prettier");`

## Extend

To extend/override this config, import it into `.prettierrc.js` like so:

```js
module.exports = {
  ...require("@sc-way/config-prettier"),
  // your overrides/additions here
};

```

## Prettier and EditorConfig?

> EditorConfig's role is to configure your editor so that the code you write is already formatted while Prettier will format your already written code. This allows EditorConfig to be used in many more languages and projects than Prettier.

>Using EditorConfig will also avoid Prettier of uselessly formatting your file on save as your editor will already have done the formatting based on EditorConfig's rules. The tricky part though is to make sure Prettier and EditorConfig have the same rules without repeating your configuration in two separate files.

[Reference article](https://blog.theodo.com/2019/08/why-you-should-use-eslint-prettier-and-editorconfig-together/)

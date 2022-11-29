# prettier-config

Prettier config used at SimonGolms

![npm version](https://img.shields.io/npm/v/@golms/prettier-config?label=npm%20Version&logo=npm)
![GitHub version](https://img.shields.io/github/package-json/v/SimonGolms/prettier-config?label=Github%20Version&logo=github)
[![License: Apache-2.0](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/simongolms/prettier-config/blob/master/LICENSE)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/simongolms/prettier-config/graphs/commit-activity)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-green.svg?logo=conventional-commits)](https://conventionalcommits.org)
[![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-494949?logo=semantic-release)](https://github.com/semantic-release/semantic-release)

## Usage

Install the package using `npm`

```sh
npm install --save-dev --save-exact @golms/prettier-config
```

Create a `.prettierrc.js` file in your projects root directory and export your desired modifications.

```js
module.exports = {
  ...require("@golms/prettier-config"),
  // printWidth: 140, // to overwrite the property
};
```

[Check out the `prettier` documentation for more info on sharing configurations](https://prettier.io/docs/en/configuration.html#sharing-configurations).

## Local Development

### Install Dependencies

```sh
npm install
```

### Test

```sh
npm test
```

### Repair

This command may be useful when obscure errors or issues are encountered. It removes and recreates dependencies of your project.

```sh
npm run repair
```

### Release

Fully automated version management and package publishing via [semantic-release](https://github.com/semantic-release). It bumps the version according to conventional commits, publishes the package to npm and release a new version to GitHub.

#### Automatic Release (GitHub Action) [Recommended]

Make sure that the secrets `GITHUB_TOKEN` and `NPM_TOKEN` are available in GitHub repository.

```sh
npm run release:ci
```

#### Manual Release

Make sure that the environment variables `GITHUB_TOKEN` and `NPM_TOKEN` are set or declared in `.env` and a productive build was previously created via `npm run build`.

```sh
npm run release
```

## Author

**Simon Golms**

- Digital Card: `npx simongolms`
- Github: [@golms](https://github.com/SimonGolms)
- Website: [gol.ms](https://gol.ms)

## Show your support

Give a ⭐️ if this project helped you!

## License

Copyright © 2022 [Simon Golms](https://github.com/simongolms).<br />
This project is [MIT](https://github.com/simongolms/homekit-code/blob/master/LICENSE) licensed.

## Resources

- https://prettier.io/

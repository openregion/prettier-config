# Prettier shared config
Open Region Prettier shared config

## Usage
Install package

```shell
npm install --save-dev @openregion/prettier-config
```

Create `.prettierrc.mjs` file with this content

```javascript
import openRegionPrettierConfig from '@openregion/prettier-config';

export default {
  ...openRegionPrettierConfig,
};
```

### ESLint
To use this package with ESLint, install

```shell
npm install --save-dev eslint-config-prettier
```

Extend ESLint config (`.eslintrc`) with `prettier`. Example:

```json
{
  "extends": [
    "@openregion",
    "prettier"
  ]
}
```

This will turn off all rules that are unnecessary or might conflict with Prettier.

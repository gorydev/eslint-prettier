\*\*\* Installation and configuration for ESLint and Prettier

Extensions: `eslint prettier``

Dependencies:
`npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node`

Now if you want airbnb style you need to install:
`npx install-peerdeps --dev eslint-config-airbnb`

https://github.com/airbnb/javascript

Now you need to create the .prettierrc config file and set the options you want :
https://prettier.io/docs/en/options.html

Create the .eslintrc.js config file and set the rules you want:
https://eslint.org/docs/rules/

Or you can generate it with `eslint --init` if you installed eslint it globally:

```json
{
  "extends": ["airbnb", "prettier", "plugin:node/recommended"],
  "plugins": ["prettier"],
  "rules": {
    "prettier/prettier": "error",
    "no-unused-vars": "warn",
    "no-console": "off",
    "func-names": "off",
    "no-process-exit": "off",
    "object-shorthand": "off",
    "class-methods-use-this": "off"
  }
}
```

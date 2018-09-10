# dedent.macro

A [babel macro](https://github.com/kentcdodds/babel-plugin-macros) for [dedent](https://yarn.pm/dedent)

## Usage

### Setting up babel macros

```
yarn add babel-plugin-macros
```

**.babelrc**

```
{
  "plugins": ["macros"]
}
```

See more info in the [main documentation](https://github.com/kentcdodds/babel-plugin-macros/blob/master/other/docs/user.md)

### Setting up `dedent.macro`

```
yarn add --dev dedent.macro
```

```js
import dedent from 'dedent.macro'

    dedent`
    hi there
    this is fine
    `
```

This will transform out the leading spaces, just like regular Dedent usage would, but with the difference being that the dedent call will be transformed out completely during the babel process.

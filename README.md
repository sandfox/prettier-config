# Prettier Config

read prettier ops from a `.prettieropts` file

npm-ed version of https://gist.github.com/epeli/7e9511cbd2ec806c5f8a6f96428352c2

requires `prettier` to be installed.

```
npm install --save-dev prettier-config
```

Currently known to only work when when used inside a script inside `package.json`.
This is because it has no idea how to find the `prettier` binary without npm doing the work for it.
Could be made to work via a global install.

e.g
```
{
  "scripts": {
    "fmt": "prettier-config \"lib/**/*.js\"",
    "check": "prettier-config --list-different \"lib/**/*.js\""
  }
}
```

```
npm run fmt
yarn fmt
```
>>>>>>> initial commit

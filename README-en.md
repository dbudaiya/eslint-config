# @dushenyan/eslint-config

[![npm](https://img.shields.io/npm/v/@dushenyan/eslint-config?color=a1b858&label=)](https://npmjs.com/package/@dushenyan/eslint-config)

- Single quotes, no semi
- Auto fix for formatting (aimed to be used standalone without Prettier)
- TypeScript, Vue, React out-of-box
- Lint also for json, yaml, markdown
- Sorted imports, dangling commas for cleaner commit diff
- Reasonable defaults, best practices, only one-line of config

## Usage

### Install

```bash
pnpm add -D eslint @dushenyan/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends": "@dushenyan"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## Check Also

- [dushenyan/dotfiles](https://github.com/dushenyan/dotfiles) - My dotfiles
- [dushenyan/vscode-settings](https://github.com/dushenyan/vscode-settings) - My VS Code settings
- [dushenyan/eslint-config](https://github.com/dushenyan/eslint-config) - My ESLint config
- [dushenyan/ts-starter](https://github.com/dushenyan/ts-starter) - My starter template for TypeScript library
- [dushenyan/vitesse](https://github.com/dushenyan/vitesse) - My starter template for Vue & Vite app

## License

MIT

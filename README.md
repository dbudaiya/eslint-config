# @dushenyan/eslint-config

- 单引号，没有半引号
- 自动修复格式化（旨在在没有 Prettier 的情况下独立使用）
- TypeScript、Vue、React 开箱即用
- Lint 也适用于 json、yaml、markdown
- 排序导入，悬空逗号以获得更清晰的提交差异
- 合理的默认值，最佳实践，只有一行配置

## 使用

### 安装

```bash
pnpm add -D eslint @dushenyan/eslint-config
```

### 配置 `.eslintrc`

```json
{
  "extends": "@dushenyan"
}
```

> 通常不需要`.eslintignore`，因为它已由预设提供。

### 添加文件 package.json

例子:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### 配置 VS 代码自动修复

添加文件 `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## License

MIT

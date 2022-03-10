# eslint-config

## Usage

```Install
# @ouduidui/eslint-config-basic : for javascript
pnpm i -D eslint @ouduidui/eslint-config-basic

# @ouduidui/eslint-config-ts : for typescript
pnpm i -D eslint @ouduidui/eslint-config-ts

# @ouduidui/eslint-config-vue : for Vue
pnpm i -D eslint @ouduidui/eslint-config-vue

# @ouduidui/eslint-config-react : for React
pnpm i -D eslint @ouduidui/eslint-config-react

```

### Config `.eslintrc`

```json
{
  "extends": ["@ouduidui/eslint-config-basic"]
}
```

### Config `.eslintignore`

```txt
dist
public
```

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint \"**/*.{vue,ts,js}\""
  }
}
```

### Config VSCode auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

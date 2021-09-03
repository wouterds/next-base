# web

![code-review](https://github.com/wouterds/next-base/workflows/code-review/badge.svg?branch=main)
![docker-image](https://github.com/wouterds/next-base/workflows/docker-image/badge.svg?branch=main)
![deploy](https://github.com/wouterds/next-base/workflows/deploy/badge.svg?branch=main)

## Development

```bash
# switch node version
nvm install

# install dependencies
yarn

# start development environment
yarn dev
```

### VSCode

#### Plugins

- https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint
- https://marketplace.visualstudio.com/items?itemName=stylelint.vscode-stylelint
- https://marketplace.visualstudio.com/items?itemName=cpylua.language-postcss

#### Workspace settings

```javascript
{
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact"
  ],
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.fixAll.stylelint": true,
  },
  "files.associations": {
    "*.css": "postcss",
  },
}
```

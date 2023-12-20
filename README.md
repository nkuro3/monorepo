# momorepo default settings

### reference

[Create a monorepo using PNPM workspace](https://dev.to/vinomanick/create-a-monorepo-using-pnpm-workspace-1ebn)

### memo

I changed from above reference like below.

1. change sttings.json to enable auto format on save

   ```json
   {
     "editor.formatOnSave": true,
     "editor.defaultFormatter": "esbenp.prettier-vscode",
     // add
     "editor.codeActionsOnSave": {
       "source.fixAll.eslint": "explicit"
     }
   }
   ```

2. delete `.eslintrc.cjs` from apps/web-app to enable lint

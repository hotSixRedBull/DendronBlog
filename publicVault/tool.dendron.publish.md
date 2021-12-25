---
id: PxclDrzGSLcuth6AKovQi
title: Publish
desc: ''
updated: 1640448168272
created: 1640184615528
---

Referred [this guide](https://wiki.dendron.so/notes/yg3EL1x9fEe4NMqxUC3jP/).

## Setup
### NPM
In root folder,
```
npm init -y 
npm install -g @dendronhq/dendron-cli@latest
echo .next >> .gitignore
npx dendron publish init
```

### YAML
- Run `Dendron: Configure (yaml)` command.
- publishing the repo named kevinslin.github.io
```
site:
    siteUrl: https://kevinslin.github.io
```
- publishing the repo named dendron-publish-sample
```
site:
    assetsPrefix: /dendron-publish-sample
    siteUrl: https://kevinslin.github.io
```

### Build
```
npx dendron publish dev
```

### Publish
- Run your vscode as administrator.
```
dendron publish export --target github
```
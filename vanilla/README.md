# パッケージインストール

```
$ docker-compose exec node bash
$ cd /docker/vanilla/
$ yarn install
```

# ビルド

```
$ docker-compose exec node /docker/vanilla/node_modules/typescript/bin/tsc /docker/vanilla/index.ts
```

# 実行

```
$ docker-compose exec node node /docker/vanilla/index.js
```

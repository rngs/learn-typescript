# パッケージインストール

```
$ docker-compose exec node bash
$ cd /docker/vanilla/
$ yarn install
```

# ビルド

```
$ docker-compose exec node /docker/vanilla/node_modules/typescript/bin/tsc
```

# 実行

```
$ docker-compose exec node node /docker/vanilla/index.js
```

# tsconfig

## initialize

```
$ docker-compose exec node bash

$ cd /docker/vanilla
$ node_modules/typescript/bin/tsc --init
```

## トランスパイル元/先を変更

```json
"compilerOptions": {
    "outDir": "./dist/js", //トランスパイル先
    "rootDir": "./src/ts", //対象ディレクトリ
}
```

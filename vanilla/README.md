# 前提

- コンテナに入っていること
    ```
    $ docker-compose exec node bash
    $ cd /docker/vanilla/
    ```

# パッケージインストール

```
$ yarn install
```

# ビルド

```
$ ./node_modules/typescript/bin/tsc
```

# 実行

```
$ node ./dist/js/index.js
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

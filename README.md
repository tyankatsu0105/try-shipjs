shipjsの検証用

# 分かったこと
- 最初の一回は自分でタグ打たないと動かない
  - `git release patch`とかでタグ打ってcommitして、それらをpush priginすれば以降は問題ない
- ~~`conventional-changelog`を使用するので、それをインストールしておかないとだめ~~
  - 関係なかった node_modules/shipjs/node_modules/.bin/conventional-changelogなので、shipjsが持ってる
- yarnだとうまくいくかもしれない
  - npmだとエラーが出る
```bash
$ /Users/tyankatsu/project/try-shipjs/node_modules/shipjs/node_modules/.bin/conventional-changelog -p angular -i CHANGELOG.md -s
/bin/sh: /Users/tyankatsu/project/try-shipjs/node_modules/shipjs/node_modules/.bin/conventional-changelog: No such file or directory
Error: {
  "message": "Exit code is 127",
  "command": "/Users/tyankatsu/project/try-shipjs/node_modules/shipjs/node_modules/.bin/conventional-changelog -p angular -i CHANGELOG.md -s",
  "result": ""
}
```
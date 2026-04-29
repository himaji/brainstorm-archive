# brainstorm-archive

`brainstorm-publish` スキルが生成するブレインストーミング HTML の置き場です。

- 各ページは `2026-04-29-{slug}-{hash}/index.html` に配置されます。
- 全ページに `<meta name="robots" content="noindex,nofollow">` が入っており、検索エンジンには載りません。
- 共有方法は **URL を直接渡す** だけです。
- ルートの `index.html` はダミーです。一覧は提供しません。

## 公開ページの URL 形式

```
https://himaji.github.io/brainstorm-archive/{YYYY-MM-DD}-{slug}-{hash}/
```

ハッシュ部分は16文字の base36 ランダム文字列で、推測は事実上不可能です。

## 自分用の一覧

ローカルの `~/.brainstorm-archive-index.json` に追記されます。

## 削除

```
git rm -r 2026-04-29-{slug}-{hash}
git commit -m "remove ..."
git push
```

## ライセンス・注意

- リポジトリ自体は public です。誤って機密情報を含めないこと。
- 公開ページの URL を知っている人は誰でもアクセスできます。

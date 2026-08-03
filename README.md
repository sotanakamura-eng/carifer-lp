# Carifer LP

株式会社TLの若手向けキャリア支援サービス「Carifer」の公開ランディングページです。

## Claude Codeで編集する

```bash
git clone https://github.com/sotanakamura-eng/carifer-lp.git
cd carifer-lp
claude
```

このリポジトリは、追加のインストールなしで編集できる静的サイトです。Claude Codeには次のように依頼してください。

```text
CLAUDE.mdを確認してからindex.htmlを編集してください。
既存のデザインとスマホ対応を保ち、変更後にブラウザ表示を確認してください。
```

主なファイル：

- `index.html` — ページ内容とCSSを含む公開サイト本体
- `og.png` — SNS共有用画像
- `CLAUDE.md` — Claude Code向け編集ルール

ローカル確認は、リポジトリ内で次を実行します。

```bash
python3 -m http.server 8000
```

その後 `http://localhost:8000` を開きます。`main` ブランチへ変更をpushすると、GitHub Pagesが自動更新されます。

## 公開URL

https://sotanakamura-eng.github.io/carifer-lp/

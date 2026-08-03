# Carifer LP

株式会社TLの若手向けキャリア支援サービス「Carifer」のランディングページです。

## Claude Codeで編集する

```bash
git clone https://github.com/sotanakamura-eng/carifer-lp.git
cd carifer-lp
npm install
npm run dev
```

ブラウザで `http://localhost:3000` を開きます。主な編集対象は次の2ファイルです。

- `app/page.tsx` — ページの文章・セクション構成
- `app/globals.css` — 色・余白・レスポンシブを含むデザイン

Claude Codeには、たとえば次のように依頼できます。

```text
CLAUDE.mdを確認してから、Cariferのファーストビューの文章を変更してください。
変更後にnpm run buildで確認してください。
```

## 公開用ファイルを更新する

```bash
npm run build
npm run start
```

別のターミナルで次を実行すると、`github-pages/` に静的版が生成されます。

```bash
node scripts/build-github-pages.mjs
```

GitHub Pagesは `main` ブランチ直下の `index.html` を公開しています。生成した
`github-pages/index.html` をルートの `index.html` として反映してください。

## 動作環境

- Node.js 22.13以上
- npm

## 確認コマンド

```bash
npm run build
npm test
```

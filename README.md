# toujishaishiki.jp

当事者意識をテーマにしたシンプルな静的ウェブサイト。Cloudflare Workers の静的アセット機能でホスティングします。

## 構成

```
.
├── public/          静的ファイル（このディレクトリが配信される）
│   ├── index.html
│   └── style.css
├── wrangler.jsonc   Cloudflare Workers の設定
└── package.json
```

## セットアップ

```sh
npm install
```

## ローカルで確認

```sh
npm run dev
```

ブラウザで http://localhost:8787 を開きます。

## デプロイ

初回のみ Cloudflare にログインします。

```sh
npx wrangler login
```

デプロイ：

```sh
npm run deploy
```

公開先 URL（`https://toujishaishiki-jp.<account>.workers.dev`）が表示されます。

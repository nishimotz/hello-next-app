# hello-next-app

This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## 作業履歴

プロジェクト名のフォルダが作成される。

```bash
npx create-next-app@latest
```

オプションはすべてデフォルトのまま。

```text
✔ What is your project named? … hello-next-app
✔ Would you like to use TypeScript? … No / Yes
✔ Would you like to use ESLint? … No / Yes
✔ Would you like to use Tailwind CSS? … No / Yes
✔ Would you like your code inside a `src/` directory? … No / Yes
✔ Would you like to use App Router? (recommended) … No / Yes
✔ Would you like to use Turbopack for next dev? … No / Yes
✔ Would you like to customize the import alias (@/* by default)? … No / Yes
```

```bash
cd hello-next-app
npm run dev
```

## Static Exports

[Static Exports](https://nextjs.org/docs/app/building-your-application/deploying/static-exports)

next.config.ts に output: 'export' を追加。

```bash
npx next build
python3 -m http.server -d out
```

ブラウザで `http://0.0.0.0:8000/` にアクセスすると、ビルドしたファイルが表示される。

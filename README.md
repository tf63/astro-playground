# Astro Playground

## 備忘録

### セットアップ

**プロジェクトの作成**

```shell
pnpm create astro@latest
```

**インテグレーションの追加**

- https://docs.astro.build/ja/guides/integrations-guide/

```shell
pnpm astro add react
pnpm astro add tailwind
```

**path aliasの指定**
`tsconfig.json`でbaseUrlとpathsを指定する

```
    "baseUrl": ".",
    "paths": {
        "@/*": ["./src/*"]
    }
```

### Vite

AstroはViteを使ってるっぽい

- https://docs.astro.build/ja/recipes/add-yaml-support/

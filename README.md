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

`astro.config.mjs`にインテグレーションが生える

```javascript
import react from '@astrojs/react'
import tailwind from '@astrojs/tailwind'
import { defineConfig } from 'astro/config'

// https://astro.build/config
export default defineConfig({
    integrations: [tailwind(), react()],
})
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

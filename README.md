A Simple Preset for unplugin-auto-import.

## Quick Start (Vite)

```ts
// vite.config.ts
import { defineConfig } from 'vite'
import AutoImport from 'unplugin-auto-import/vite'
import { ElementPlusResolver } from 'unplugin-vue-components/resolvers'
import ElementPlusPreset from 'unplugin-auto-import-element-plus-preset'

export default defineConfig({
    ...
    plugins: [
        ...
        AutoImport({
            imports: [
                ElementPlusPreset
            ],
            resolvers: [
                ElementPlusResolver()
            ]
        })
    ]
})
```
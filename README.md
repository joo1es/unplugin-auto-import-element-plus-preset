A Simple Preset for unplugin-auto-import.

## Use type.d.ts

tsconfig.json

```json
{
    "compilerOptions": {
        ...
        "types": [
            ...
            "unplugin-auto-import-element-plus-preset/type"
        ]
    }
}
```

## Use Preset (No Style)

```ts
// vite.config.ts
import { defineConfig } from 'vite'
import AutoImport from 'unplugin-auto-import/vite'
import ElementPlusPreset from 'unplugin-auto-import-element-plus-preset'

export default defineConfig({
    ...
    plugins: [
        ...
        AutoImport({
            imports: [
                ElementPlusPreset
            ]
        })
    ]
})
```

```ts
// <script lang="ts" setup>
const schemas = [
    {
        prop: 'text',
        component: ElInput // don't need to care tsc error
    }
]
```
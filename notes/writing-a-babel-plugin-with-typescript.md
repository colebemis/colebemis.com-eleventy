---
title: Writing a Babel plugin with TypeScript
date: 2021-07-30T20:39:31.591Z
---
```ts
import { PluginObj } from '@babel/core'
import * as babel from '@babel/core'

export default function ({ types: t }: typeof babel): PluginObj {
  return {
    visitor: {...},
    },
  }
}
```
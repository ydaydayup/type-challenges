## Play Locally

You can build the challenges and play locally using your preferred IDE or text editor with TypeScript language support.

To do that, you will need the latest version of [Node.js](https://nodejs.org/) and [pnpm](https://pnpm.io/) installed.

After cloning the repo, installed the dependencies by:

```bash
pnpm install
```

Then and run the `generate` script:

```bash
pnpm generate
```

It will prompt you to select the desired language, then you can find the generated challenges in the `./playground` folder.

Later if you want to update playground while keeping your changes:

```bash
pnpm generate --keep-changes
```
OR
```bash
pnpm generate -K
```

note:
1. 报错如下
```bash
 pnpm generate                                                                                                                                                                                                                                                 21:11:46

> type-challenges@0.0.0 generate /Users/yunhongze/Documents/code/type-challenges
> esno ./scripts/generate-play.ts

(node:17900) ExperimentalWarning: Custom ESM Loaders is an experimental feature and might change at any time
(Use `node --trace-warnings ...` to show where the warning was created)
/Users/yunhongze/Documents/code/type-challenges/scripts/generate-play.ts:1
import path from 'path'
^^^^^^

SyntaxError: Cannot use import statement outside a module
    at internalCompileFunction (node:internal/vm:73:18)
    at wrapSafe (node:internal/modules/cjs/loader:1153:20)
    at Module._compile (node:internal/modules/cjs/loader:1197:27)
    at Module._extensions..js (node:internal/modules/cjs/loader:1287:10)
    at Module.load (node:internal/modules/cjs/loader:1091:32)
    at Module._load (node:internal/modules/cjs/loader:938:12)
    at ModuleWrap.<anonymous> (node:internal/modules/esm/translators:165:29)
    at ModuleJob.run (node:internal/modules/esm/module_job:192:25)
    at async CustomizedModuleLoader.import (node:internal/modules/esm/loader:228:24)
    at async loadESM (node:internal/process/esm_loader:40:7)

Node.js v20.5.1

```

> 如果版本是20是会报错的
> 请使用如下命令使用18.17.1
> pnpm env use --global lts
> pnpm env list                                                                                                                                                                                                           ✘  21:34:19
  18.17.1


# Plugins

Add or customize features through plugins.

Currently, plugins can only be manually added at build time and they are not dynamically imported. In the future, this will change.

## Layout

Always a `package.json`, `tsconfig.json`. And, an `_isomorphic.ts` file, along with a `_client.ts` and/or a `_server.ts`.

With contents like:

```jsonc
// package.json
{
	"name": "@quasipanacea/plugin,<resourceType>.<id>.(controller|view).<optionalExtra>",
	"dependencies": {
		"@quasipanacea/common": "workspace:^",
		"@quasipanacea/plugin-utility": "workspace:^"
	},
	"devDependencies": {
		"vue": "^3.0.0",
		"vue-router": "^4.0.0"
	},
	"peerDependencies": {
		"vue": "^3.0.0",
		"vue-router": "^4.0.0"
	}
}
```

```jsonc
// tsconfig.json
{
	"extends": "@quasipanacea/common/tsconfig.json"
}
```

```ts
// client.ts
import { pluginServer } from '@quasipanacea/common/server/index.ts'

import { metadata, format } from './_isomorphic.ts'
import { default as component } from './<PluginFamily><Id>.vue'

export async function init() {
	pluginServer.register({
		metadata,
		podView: {
			format,
			component,
		},
	})
}
```

```ts
// server.ts
import { pluginServer } from '@quasipanacea/common/server/index.ts'

import { metadata, format } from './_isomorphic.ts'
import * as Exports from './<pluginFamily><Id>.ts'

export async function init() {
	pluginServer.register({
		metadata,
		format,
		podController: {
			...Exports,
		},
	})
}
```

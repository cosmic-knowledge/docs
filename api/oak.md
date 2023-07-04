# Oak

In your backend file:

```ts
import { Router, send } from 'oak/mod.ts'

export const oakRouter = new Router().get(
	'/some-route/:value',
	async (ctx: Router) => {
		const value = ctx.params.value

		console.log(value)
	},
)
```

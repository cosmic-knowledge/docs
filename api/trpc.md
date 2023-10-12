# tRPC

In your backend file:

```ts
import * as path from 'node:path'
import { z } from 'zod'

export const trpcRouter = trpc.router({
	customRoute: pluginProcedure
		.input(
				z.object({
					value: z.string()
				}),
			)
			.output(z.void())
			.mutation(async ({ ctx, input }) => {
				await Deno.writeTextFile(ctx.state.myFile, value)
			}),
})
```

# Popup

For now, typings is limited to internal plugins at `common/client/popup.ts`. In this future, this will change.

## To show

```ts
import { popup } from '@quasipanacea/common/client/index.js'
import { ViewCreatePopup } from '@quasipanacea/common/components/index.js'

await popup.show('view-create', ViewCreatePopup, {
	modelUuid: props.uuid,
})
```

## To hide

```ts
import { popup } from '@quasipanacea/common/client/index.js'

popup.hideNoData('null')
```

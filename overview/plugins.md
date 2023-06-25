# Plugins

Quasipanacea is highly extensible. There are different families:

- model
- view
- overview
- pack
- pod
- theme

The most developed plugins are:

- `quasipanacea-overview-graph`
- `quasipanacea-pod-latex`
- `quasipanacea-pod-markdown`

## API

### Popups

In your component:

```ts
import { popup } from '@quasipanacea/common/client/index.js'
import { ViewCreatePopup } from '@quasipanacea/components/index.js'

await popup.show('view-create', ViewCreatePopup, {
	modelUuid: props.uuid,
})
```

For now, you must also add the schema to `popup.ts`.

If you are adding a popup, be sure to add at least the following to close the popup:

```js
import { popup } from '@quasipanacea/common/client/index.js'

popup.hideNoData('null')
```

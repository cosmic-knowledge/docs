# Plugins

Currently, most work is confined to plugins. The most developed plugins are:

- `quasipanacea-overview-graph`
- `quasipanacea-pod-latex`
- `quasipanacea-pod-markdown`

## Popups

In your component:

```ts
import { showPopup } from '@quasipanacea/common/client/popup.js'
import { ViewCreatePopup } from '@quasipanacea/plugin-components/popups/index.js'

await showPopup('view-create', ViewCreatePopup, {
  modelUuid: props.uuid,
})
```

For now, you must also add the schema to `popup.ts`.

If you are adding a popup, be sure to add at least the following to close the popup:

```js
import { hidePopupNoData } from '@quasipanacea/common/client/popup'

hidePopupNoData('null')
```

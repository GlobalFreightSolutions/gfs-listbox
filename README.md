## GFS Listbox
`<gfs-listbox>` is a interactive list listbox.

### Install

```bash
$ npm i --save @gfsdeliver/gfs-listbox
```

### Import In a HTML file:

```html
<html>
    <head>
        <script type="module">
            import '@gfsdeliver/gfs-listbox/gfs-listbox.js';
        </script>
    </head>
    <body>
        <gfs-listbox>
            <gfs-item>Item</gfs-item>
        </gfs-listbox>
    </body>
</html>
```

### In a Polymer 3 element
```js
import { PolymerElement, html } from '@polymer/polymer/polymer-element.js';
import '@gfsdeliver/gfs-listbox/gfs-listbox.js';

class CustomElement extends PolymerElement {
    static get template() {
        return html`
            <gfs-listbox>
                <gfs-item>Item</gfs-item>
            </gfs-listbox>
        `;
    }
}
customElements.define('custom-element', CustomElement);
```

## Styling
Custom property | Description | Default
----------------|-------------|----------
--gfs-listbox | Mixin applied to the listbox | {}


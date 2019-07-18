## Installation
Due to a bug on `iron-overlay-backdrop`, if you want to override the styles, you must add them in the root file (ex. index.html).
This effect projects that start with polymer-starter-kit

Read more for the bug here:
https://github.com/Polymer/polymer-starter-kit/issues/154

## Properties
Property | Description
---------|-------------
header   | dialog header, wrapped on a "h2" element tag
body     | dialog content, wrapped on a "p" element tag

## Example

```html
<gfs-dialog id="myDialog" modal>
    <div>
        <gfs-button dialog-dismiss>Cancel</gfs-button>
        <gfs-button dialog-dismiss>Delete</gfs-button>
    </div>
</gfs-dialog>

<script>
    this.$.myDialog.header = "Dialog Header";
    this.$.myDialog.body = "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor...";
</script>

```

------------------------------------------------------------------------------------------------------------------

```html
<gfs-dialog id="myDialog" modal>
    <h2>Dialog Header</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor...</p>

    <div>
        <gfs-button dialog-dismiss>Cancel</gfs-button>
        <gfs-button dialog-dismiss>Delete</gfs-button>
    </div>
</gfs-dialog>
```

## Styling
Custom property | Description | Default
----------------|-------------|----------
--gfs-dialog-min-width | Dialog min width size | `300px`
--gfs-dialog-width | Dialog with size | `auto`
--gfs-dialog-max-width | Dialog max with size | `600px`
--gfs-dialog-background | Dialog main background color | `#fff`
--gfs-dialog-border-radius | Dialog radius corners | `3px`
--gfs-dialog-header-color | Dialog color | `#000`
--gfs-dialog-header-background | Dialog color | `var(--gfs-dialog-background)`

### Example
```html
<style>
    #myDialog {
        --gfs-dialog-min-width: 300px;
        --gfs-dialog-width: auto;
        --gfs-dialog-max-width: 600px;
        --gfs-dialog-background: red;
        --gfs-dialog-border-radius: 15px;
        --gfs-dialog-header-color: var(--gfs-secondary-color);
    }
</style>
```

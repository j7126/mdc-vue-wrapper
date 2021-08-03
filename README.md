# mdc-vue-wrapper

A basic wrapper to use material components with vuejs

Currently a work in progress, many components are not implemented or are missing features.

## Install

This depends on vue and material-components-web. 

mdc-vue-wrapper can be used with the cdn versions of vue and material-components-web, or it can be used with the locally imported modules with Sass and ES2015, compiled with webpack. 

```js
import 'mdc-vue-wrapper'
```
or
```js
import '/path/to/mdc-vue-wrapper.js'
```
or
```html
<script src="/path/to/mdc-vue-wrapper.js"></script>
```


## Components

### Top App Bar

#### Example

```html
<mdc-top-app-bar title="Title">
    <template slot="end">
        <!-- Right aligned content -->
    </template>
</mdc-top-app-bar>
```

#### Props

| Prop | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| `title` | String | false | `''` | Title text |

#### Slots

| Slot | Description |
|------|-------------|
| `end` | Content in the end section

### Button

#### Example

```html
<mdc-button raised @click="clickHandler">
    Button Text
</mdc-button>
```

#### Props

| Prop | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| `outlined` | Bool | false | `false` | Outline button style. Incompatible with `raised` and `unelevated` |
| `raised` | Bool | false | `false` | Elevated button style. Incompatible with `outlined` and `unelevated` |
| `unelevated` | Bool | false | `false` | Flat button style. Incompatible with `outlined` and `raised` |
| `Icon` | String | false | `null` | The material-icons name for the icon |
| `disabled` | Bool | False | `false` | Disable the button |

#### Events

| Event | Payload | Description |
|-------|---------|-------------|
| `Click` | none | Fired when the button is clicked |

#### Slots

| Slot | Description |
|------|-------------|
| `default` | Button Content |

### Floating Action Button

#### Example

```html
<mdc-fab icon="add" @click="clickHandler" />
```

#### Props

| Prop | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| `Icon` | String | true | `null` | The material-icons name for the icon |

#### Events

| Event | Payload | Description |
|-------|---------|-------------|
| `Click` | none | Fired when the button is clicked |

### Icon Button

#### Example

```html
<mdc-icon-button icon="add" @click="clickHandler" />
```

#### Props

| Prop | Type | Required | Default | Description |
|------|------|----------|---------|-------------|
| `Icon` | String | true | `null` | The material-icons name for the icon |

#### Events

| Event | Payload | Description |
|-------|---------|-------------|
| `Click` | none | Fired when the button is clicked |

### Switch

### Checkbox

### Text Field

### Select

### Select Option

### Dialog

### Card

### Typography
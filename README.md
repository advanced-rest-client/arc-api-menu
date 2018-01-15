[![Build Status](https://travis-ci.org/advanced-rest-client/arc-api-menu.svg?branch=stage)](https://travis-ci.org/advanced-rest-client/arc-api-menu)  

# arc-api-menu

ARC menu for APIs includes ARC projects menu and the REST APIs menu.

The REST APIs menu is disabled by default. To enable it set `rest-api`
attribute on the element. Once set it displays tabs view to switch between ARC
projects and REST APIs lists.

### Example
```
<arc-api-menu rest-api></arc-api-menu>
```

### Styling
`<arc-api-menu>` provides the following custom properties and mixins for styling:

Custom property | Description | Default
----------------|-------------|----------
`--arc-api-menu` | Mixin applied to the element | `{}`
`--arc-api-menu-actions-container` | Mixin applied to actions container at the bottom of REST APIs menu | `{}`

### Sizing

The element needs to be sized be setting a height. It uses vertical flex layout
so if the height is not set then it renders as a `0px` height element when the list
is empty.



### Events
| Name | Description | Params |
| --- | --- | --- |
| navigate | Dispatched when the user requested to open rest-projects screen. | base **String** - Currently only `rest-projects` |

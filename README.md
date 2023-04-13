Svelte Material Icon Component
==============================

This component allows you to easily display Material Icons in your Svelte app.

Installation
------------

You can install this component using npm:

`npm install meticon`

Usage
-----

Import the component and use it in your Svelte template:


```svelte
<script> 
import Icon from "meticon";

  let iconName = "favorite";
  let iconType = "filled";
  let className = "";
  let style = ""; 
</script>

<Icon name={iconName} type={iconType} class={className} style={style} />
```

### Props

-   `name` (required): The name of the Material Icon to display.
-   `type` (optional): The style of the Material Icon. Can be one of `"filled"`, `"outlined"`, `"round"`, `"sharp"`, or `"two-tone"`. Defaults to `"outlined"`.
-   `class` (optional): A string of additional CSS classes to apply to the icon element.
-   `style` (optional): A string of inline CSS styles to apply to the icon element.

### Font Files

This component relies on the Material Icons font files, which are not included in this package. You can either host the font files yourself and update the `@font-face` rule in the component's stylesheet, or use a CDN. The example code in this readme uses a CDN to load the font files.

Styling
-------

You can customize the styling of the Material Icons by modifying the styles in the component's stylesheet. The default styles include support for WebKit browsers, Safari and Chrome, Firefox, and IE. The stylesheet also includes classes for each icon style (`"filled"`, `"outlined"`, `"round"`, `"sharp"`, and `"two-tone"`) that you can use to further customize the appearance of the icons.
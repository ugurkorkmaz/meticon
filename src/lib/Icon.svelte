<script lang="ts">
  let className = "";
  let iconName = "";
  let iconType: "filled" | "outlined" | "round" | "sharp" | "two-tone" = "filled";
  let style = "";
  export { className as class, iconName as name, iconType as type, style };
</script>

<i
  translate="no"
  class="select-none material-icons {iconType} {className}"
  {style}
>
  {iconName}
</i>

<style>
  @font-face {
    font-family: "Material Icons";
    font-style: normal;
    font-weight: 400;
    src: url(https://example.com/MaterialIcons-Regular.eot); /* For IE6-8 */
    src: local("Material Icons"), local("MaterialIcons-Regular"),
      url(https://example.com/MaterialIcons-Regular.woff2) format("woff2"),
      url(https://example.com/MaterialIcons-Regular.woff) format("woff"),
      url(https://example.com/MaterialIcons-Regular.ttf) format("truetype");
  }
  .select-none {
    user-select: none;
  }
  .material-icons {
    font-family: "Material Icons";
    font-weight: normal;
    font-style: normal;
    font-size: 24px; /* Preferred icon size */
    display: inline-block;
    line-height: 1;
    text-transform: none;
    letter-spacing: normal;
    word-wrap: normal;
    white-space: nowrap;
    direction: ltr;

    /* Support for all WebKit browsers. */
    -webkit-font-smoothing: antialiased;
    /* Support for Safari and Chrome. */
    text-rendering: optimizeLegibility;

    /* Support for Firefox. */
    -moz-osx-font-smoothing: grayscale;

    /* Support for IE. */
    font-feature-settings: "liga";
  }
  .material-icons.filled {
    font-family: "Material Icons";
  }
  .material-icons.outlined {
    font-family: "Material Icons Outlined";
  }
  .material-icons.round {
    font-family: "Material Icons Round";
  }
  .material-icons.sharp {
    font-family: "Material Icons Sharp";
  }
  .material-icons.two-tone {
    font-family: "Material Icons Two Tone";
  }
</style>

<script lang="ts">
  import Icon from "$lib/Icon.svelte";

  const og_image = "https://opengraph.githubassets.com/a974346ea8702243b4e5892f20f0017ccf0072fac3962c6ba39ed85bbdd9da5e/ugurkorkmaz/meticon";
</script>

<svelte:head>
  <title>Meticon</title>
  <meta name="twitter:image:src" content={og_image} />
  <meta name="twitter:site" content="@ugurkorkmaz" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="ugurkorkmaz/meticon: A Google material icon library for Svelte" />
  <meta name="twitter:description" content="A Google material icon library for Svelte. Contribute to ugurkorkmaz/meticon development by creating an account on GitHub." />
  <meta property="og:image" content={og_image} />
  <meta property="og:image:alt" content="A Google material icon library for Svelte. Contribute to ugurkorkmaz/meticon development by creating an account on GitHub." />
  <meta property="og:image:width" content="1200" />
  <meta property="og:image:height" content="600" />
  <meta property="og:site_name" content="Meticon" />
  <meta property="og:type" content="object" />
  <meta property="og:title" content="ugurkorkmaz/meticon: A Google material icon library for Svelte" />
  <meta property="og:url" content="https://meticon.ugurkorkmaz.net" />
  <meta property="og:description" content="A Google material icon library for Svelte. Contribute to ugurkorkmaz/meticon development by creating an account on GitHub." />
</svelte:head>

<div class="wrapper">
  <div class="show">
    <Icon name="person" type="filled" />
    <span>Filled</span>
  </div>
  <div class="show">
    <Icon name="person" type="outlined" />
    <span>Outlined</span>
  </div>

  <div class="show">
    <Icon name="person" type="round" />
    <span>Round</span>
  </div>

  <div class="show">
    <Icon name="person" type="sharp" />
    <span>Sharp</span>
  </div>

  <div class="show">
    <Icon name="person" type="two-tone" />
    <span>Two Tone</span>
  </div>
</div>

<style global>
  .wrapper {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  .show {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0 1rem;
    font-size: large;
  }

  .show span {
    margin-top: 1rem;
  }
</style>
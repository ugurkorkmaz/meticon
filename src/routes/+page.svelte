<script lang="ts">
  import Icon from "$lib/Icon.svelte";

  const og_image =
    "https://opengraph.githubassets.com/a974346ea8702243b4e5892f20f0017ccf0072fac3962c6ba39ed85bbdd9da5e/ugurkorkmaz/meticon";
</script>

<svelte:head>
  <title>Meticon</title>
  <meta name="twitter:image:src" content={og_image} />
  <meta name="twitter:site" content="@ugurkorkmaz" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta
    name="twitter:title"
    content="ugurkorkmaz/meticon: A Google material icon library for Svelte"
  />
  <meta
    name="twitter:description"
    content="A Google material icon library for Svelte. Contribute to ugurkorkmaz/meticon development by creating an account on GitHub."
  />
  <meta property="og:image" content={og_image} />
  <meta
    property="og:image:alt"
    content="A Google material icon library for Svelte. Contribute to ugurkorkmaz/meticon development by creating an account on GitHub."
  />
  <meta property="og:image:width" content="1200" />
  <meta property="og:image:height" content="600" />
  <meta property="og:site_name" content="Meticon" />
  <meta property="og:type" content="object" />
  <meta
    property="og:title"
    content="ugurkorkmaz/meticon: A Google material icon library for Svelte"
  />
  <meta property="og:url" content="https://meticon.ugurkorkmaz.net" />
  <meta
    property="og:description"
    content="A Google material icon library for Svelte. Contribute to ugurkorkmaz/meticon development by creating an account on GitHub."
  />
</svelte:head>

<main>
  <div class="header">
    <h1>Meticon</h1>
    <p>A Google material icon library for Svelte</p>
    <a
      href="https://github.com/ugurkorkmaz/meticon"
      class="github-button"
      aria-label="Star ugurkorkmaz/meticon on GitHub"
    >
      <Icon name="star" type="filled" class="mr-2 text-yellow-300" />
      Star on GitHub
    </a>
  </div>
  <div class="content">
    <div>
      <Icon name="person" type="filled" class="text-blue-500" />
      <span>Filled</span>
    </div>
    <div>
      <Icon name="person" type="outlined" class="text-red-500" />
      <span>Outlined</span>
    </div>
    <div>
      <Icon name="person" type="round" class="text-green-500" />
      <span>Round</span>
    </div>
    <div>
      <Icon name="person" type="sharp" class="text-purple-500" />
      <span>Sharp</span>
    </div>
    <div>
      <Icon name="person" type="two-tone" class="text-yellow-500" />
      <span>Two Tone</span>
    </div>
  </div>
</main>

<style>
  main {
    @apply flex flex-col items-center justify-center h-screen;
  }
  .header {
    @apply text-center;
    @apply mb-8;
  }
  .header > h1 {
    @apply text-4xl font-bold;
  }
  .header > p {
    @apply text-gray-500;
  }
  .header > a {
    @apply text-gray-300;
  }
  .content {
    @apply flex flex-wrap;
    @apply gap-4;
  }
  .content > div {
    @apply flex flex-col items-center;
  }
  .content > div > span {
    @apply mt-2;
  }
  .github-button {
    @apply inline-flex items-center px-4 py-2 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-gray-900 hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-500;
    @apply mt-4;
  }
</style>

<script lang="ts">
  import Icon from "$lib/Icon.svelte";
</script>

<div class="wrapper">
  <div class="show">
    <Icon name="person" type="filled"/>
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

<script>
  import Navigation from "./_navigation.svelte";

</script>

<div class="app">
  <Navigation />
  <div class="container-fluid">
    <main>
      <slot />
    </main>
  </div>
</div>

<style>
  .app {
    position: fixed;
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  .container-fluid {
    height: 100%;
    overflow: hidden;
    margin-bottom: 16px;
    flex: 1 1 0;
  }
  main {
    height: 100%;
    width: 100%;
    overflow: hidden;
  }
  :global(.page) {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }
</style>

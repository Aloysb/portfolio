<script lang="ts">
  export let name: string;
  import Navigation from "./components/Navigation/Navigation.svelte";
</script>

<div class="container">
  <Navigation />
  <main>
    <section>Illustration</section>
    <section>Projects</section>
    <section>Blog</section>
    <section>Contact</section>
  </main>
</div>

<style>
  .container {
    display: flex;
    background: var(--color-darkest);
    box-sizing: border-box;
  }

  main {
    flex: 1 1 auto;
    overflow: scroll;
    max-height: 100vh;
  }

  section {
    height: 100vh;
    border: 5px solid red;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

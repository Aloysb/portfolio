<script lang="ts">
  export let name: string;
  import Navigation from "./components/Navigation/Navigation.svelte";
</script>

<div class="container">
  <Navigation />
  <main>
    <section class="bg-red">Illustration</section>
    <section>Projects</section>
    <section>Blog</section>
    <section>Contact</section>
  </main>
</div>

<svelte:head>
  <!-- :root vars, credits to mjgarten#1939 -->
  <style>
    :root {
      --heading-border-color: yellow;
    }
  </style>
</svelte:head>

<style>
  :root {
    --color-darkest: #151515;
    --color-dark: #403d42;
    --color-light: #f3f2f3;
    --color-lightgray: #9c9a9e;
    --color-gray: #202022;
  }

  .container {
    display: flex;
    background-color: var(--color-darkest);
    color: var(--color-light);
    box-sizing: border-box;
  }

  main {
    flex: 1 1 auto;
    overflow: scroll;
    max-height: 100vh;
  }

  section {
    height: 95vh;
    border: 5px solid red;
    background-color: var(--color-gray);
    margin: 2em;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

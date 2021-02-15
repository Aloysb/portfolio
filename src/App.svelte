<script lang="ts">
  export let name: string;
  import Navigation from "./components/Navigation.svelte";
  import Section from "./components/Section.svelte";
  import ProjectCard from "./components/ProjectCard.svelte";
</script>

<div
  class="font-mono w-screen p-12 min-h-screen bg-gray-900 text-gray-50 flex items-stretch"
>
  <div class="container flex mx-auto items-stretch">
    <Navigation />
    <main class="flex-auto overflow-y-auto max-h-screen">
      <Section>
        <h1>Illustration</h1>
      </Section>
      <Section>
        <h1>Projects</h1>
        <ProjectCard title="beta" />
        <ProjectCard title="Stolen Paragliders" />
        <ProjectCard title="Aloys' dev" />
        <ProjectCard title="Doctofiche" />
      </Section>
      <Section>
        <h1>Blog</h1>
      </Section>
      <Section>
        <h1>Contact</h1>
      </Section>
    </main>
  </div>
</div>

<style>
  :root {
    --color-darkest: #151515;
    --color-dark: #403d42;
    --color-light: #f3f2f3;
    --color-lightgray: #9c9a9e;
    --color-gray: #202022;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

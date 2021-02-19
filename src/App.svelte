<script lang="ts">
  import Navigation from "./components/Navigation.svelte";
  import Section from "./components/Section.svelte";
  import ProjectCard from "./components/ProjectCard.svelte";
  import Contact from "./components/Contact.svelte";
  import Illustration from "./static/undraw_code_thinking.svelte";
</script>

<div class="font-mono w-screen min-h-screen bg-gray-900 text-gray-50 flex items-stretch">
  <Navigation />
  <main class="flex-auto overflow-y-auto max-h-screen">
    <Section id="home">
      <div class="flex flex-col items-center justify-around ">
        <div class="bg-green-500 rounded-full h-96 w-96 flex bg-opacity-75">
          <Illustration />
        </div>
        <h1>You have an app idea but you do not know how to make it come to life ?</h1>
        <h1>You have a digital project but you are lost in the technical terms ?</h1>
        <h1>
          Or you simply need a website for your business to improve your online presence ?
        </h1>
        <h1>Let me help!</h1>
        <span>Sroll to see my work</span>
      </div>
    </Section>
    <Section>
      <h1>Projects</h1>
      <div class="flex flex-col justify-around items-stretch">
        <ProjectCard title="Beta" />
        <ProjectCard title="Stolen Paragliders" />
        <ProjectCard title="FFVL Quizz" />
        <ProjectCard title="Doctofiche" />
      </div>
    </Section>
    <Section>
      <h1>Blog</h1>
    </Section>
    <Section>
      <Contact />
    </Section>
  </main>
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

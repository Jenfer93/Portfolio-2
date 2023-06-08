<script lang="ts">
  import "../lib/styles/styles.scss";
  import Hero from "../lib/components/Hero.svelte";
  import Header from "../lib/components/Header.svelte";
  import Main from "../lib/components/Main.svelte";
  import Footer from "../lib/components/Footer.svelte";
  import About from "../lib/components/About.svelte";
  import Skills from "../lib/components/Skills.svelte";
</script>

<main>
  <Hero/>
  <Header/>
  <Main/>
  <About/>
  <Skills/>
  <Footer/>
</main>

<svelte:head>
    <title>My Portfolio</title>
    <meta name="description" content="Front end developer, Jenny Feragens portfolio page, showcasing my 
    journey and work with different development languages and framework. This will hopefully be a never ending project">
</svelte:head>

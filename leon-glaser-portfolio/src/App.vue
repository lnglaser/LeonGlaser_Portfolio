<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <img alt="Leon Glaser logo" src="./assets/LGPortfolioLogo1.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  <AboutMe
    msg="I'm a developer who branched from writing stories to making software. In both disciplines, I maintain my approach by impacting people's lives in a meaningful way." />

  <ProjectSection msg="A sampling of projects I've created or contributed to." :key="project" :projects="projects" />
  <ProjectHighlight :v-for="project in projects"></ProjectHighlight>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import AboutMe from './components/AboutMe.vue'
import ProjectSection from './components/ProjectSection.vue';
import ProjectHighlight from './components/ProjectHighlight.vue';



export default {
  name: 'App',
  components: {
    // HelloWorld,
    AboutMe,
    ProjectSection,
    ProjectHighlight,

  },
  data: () => ({
    projects: [
      {
        "id": "1",
        "title": "Mill Bornes Solitaire",
        "description": "A single-player adaptation of a classic card game, built in JavaScript, HTML and CSS.",
        "link": "https://millebornessolitaire.surge.sh/"
      },

      {
        "id": "2",
        "title": "Attic",
        "description": "An app for organizing a personal comic book collection, built with javaScript, React, and CSS.",
        "link": "https://attic-comic-book-organizer.herokuapp.com/"
      },
      {
        "id": "3",
        "title": "Kohi",
        "description": "A marketplace app built around independent coffee roasters, allowing them to list and market their blends.",
        "link": "https://protected-escarpment-45651.herokuapp.com/"
      }
    ]
  })
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
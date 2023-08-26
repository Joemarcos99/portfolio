<template>
  <card-component
    title="Joseph Marcotte"
    linkedin="https://www.linkedin.com/in/joe-marcotte"
    email="joemarcos99@gmail.com"
    github="https://github.com/Joemarcos99"
    resumePath="/Joseph-Marcotte-Resume.pdf"
  />
</template>

<script>
import CardComponent from "./components/CardComponent.vue";

export default {
  name: "App",
  components: {
    CardComponent,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible:wght@400;700&display=swap");

#app {
  display: flex;
  justify-content: center;
  font-family: "Atkinson Hyperlegible";
  font-weight: 400;
  align-items: center;
  min-height: 100vh;
  background-size: cover;
  background-position: center;
  
}

body {
  margin: 0;
  background-image: url('../public/nature.jpg');
  background-size: cover; /* Adjust as needed */
  background-position: center; /* Adjust as needed */
  /* Other styling properties if needed */
}
</style>

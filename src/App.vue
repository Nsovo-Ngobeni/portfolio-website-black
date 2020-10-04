<template>
  <div>
    <MainNavBar />
    <Header />
    <About />
    <Skills />
    <Work />
  </div>
</template>

<script>
// Imports components
import Header from "./components/Header.vue";
import MainNavBar from "./components/MainNavBar.vue";
import About from "./components/About.vue";
import Skills from "./components/Skills.vue";
import Work from "./components/Work.vue";

// Export
export default {
  name: "App",
  components: {
    Header,
    MainNavBar,
    About,
    Skills,
    Work,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: var(--main-background-color);
  color: var(--main-text-color);
  font-family: RobotoMono, sans-serif;
}

:root {
  --main-background-color: #1e515d;
  --secondary-background-color: #3e6e7a;
  --emphasised-color: coral;
  --main-text-color: #fff;
  --emphasised-text-color: #ffa500;
}
</style>
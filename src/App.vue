<template>
  <div>
    <MainNavBar />
    <Header name='Nsovo' img=''/>
  </div>
</template>

<script>
  import Header from './components/Header.vue';
  import MainNavBar from './components/MainNavBar.vue';
  export default {
    name: 'App',
    components: {
      Header,
      MainNavBar
    }
  }
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
    --main-background-color: #222;
    --main-text-color: #fff;
    --emphasised-text-color:#ffa500;
  }

</style>
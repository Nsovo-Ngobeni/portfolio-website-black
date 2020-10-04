<template>
  <div>
    <img :src="imgSrc" />
    <h3>{{ title }}</h3>
    <p>{{ content }}</p>
  </div>
</template>

<script>
export default {
  name: "Tile",
  props: {
    imgSrc: String,
    title: String,
    content: String,
  },
};
</script>

<style scoped>
div {
  margin: 10vh 0 10vh 0;
  background-color: rgba(0, 0, 0, 0);
}

* {
  text-align: center;
  background-color: rgba(0, 0, 0, 0);
}

h3:after {
  content: "";
  display: block;
  width: 85%;
  margin: auto;
  height: 2px;
  background-color: var(--emphasised-color);
  margin-bottom: 20px;
  margin-top: 7.5px;
}

@media screen and (max-width: 750px) {
  div {
    margin: 2.5vh 0 2.5vh 0;
  }

  div:first-child {
    margin-top: 15vh;
  }
}
</style>
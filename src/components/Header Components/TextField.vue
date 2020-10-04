<template>
  <div id="text-box">
    <h2>{{ intro }}</h2>
    <h1>{{ header }}</h1>
    <p>{{ description }}</p>
    <a href="#">Learn More ></a>
  </div>
</template>

<script>
export default {
  name: "Text-Box",
  props: {
    intro: String,
    header: String,
    description: String,
  },
};
</script>

<style scoped>
div {
  display: grid;
  align-content: center;
  margin-left: 10%;
  background-color: rgba(0, 0, 0, 0);
}

h1,
h2 {
  font-weight: lighter;
  background-color: rgba(0, 0, 0, 0);
}

h2 {
  font-size: 125%;
}

p {
  background-color: rgba(0, 0, 0, 0);
}

a {
  margin-top: 10px;
  text-decoration: none;
  color: var(--emphasised-text-color);
  transition: font-size 0.5s;
  background-color: rgba(0, 0, 0, 0);
}

a:hover {
  font-size: 110%;
}

@media screen and (max-width: 750px) {
  div {
    margin-left: 5%;
    margin-top: 50%;
  }
}
</style>
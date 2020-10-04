<template>
  <div id="header">
    <TextField :intro="intro" :header="header" :description="description" />
    <img :src="image" />
  </div>
</template>

<script>
// Import compnent
import TextField from "./Header Components/TextField.vue";

//Import image
import image from "../assets/images/my-photo.jpg";

export default {
  name: "Header",
  props: {
    name: String,
  },
  components: {
    TextField,
  },
  data: function () {
    return {
      intro: "Hello, I'm Nsovo",
      header: "Im a website developer",
      description:
        "I'm a website developer who specialises in JavaScript, Vue.js and React.js",
      image: image,
    };
  },
};
</script>

<style scoped>
#header {
  display: grid;
  grid-template-columns: 1fr 1fr;
  align-content: center;
  margin-top: -7.5vh;
  height: 85vh;
  background-image: linear-gradient(rgba(0, 0, 0, 0.35), rgba(0, 0, 0, 0.7)),
    url("../assets/images/CodeWall.jpg");
  background-size: cover;
  background-position: centre;
}

img {
  height: 50vh;
  border-radius: 75px;
  display: block;
  margin: auto;
}

@media screen and (max-width: 750px) {
  #header {
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 1fr;
  }

  img {
    height: 25vh;
  }
}
</style>

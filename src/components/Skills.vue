<template>
  <div id="skills">
    <Tile
      :imgSrc="phoneImg"
      title="Native Programming"
      content="I am experienced with React Native and can develop elogent looking mobile apps"
    />
    <Tile
      :imgSrc="bookImg"
      title="Dedicated Learner"
      content="I am constantly learning new ways to improve my craft and bring the best possible result to the table"
    />
    <Tile
      :imgSrc="desktopImg"
      title="Web Development"
      content="I have been creating stunning websites for over a year now and they are only getting better"
    />
  </div>
</template>

<script>
import Tile from "./Skills Components/Tile.vue";
import phoneImg from "../assets/icons/phone.svg";
import desktopImg from "../assets/icons/cascading-website.svg";
import bookImg from "../assets/icons/open-book.svg";

export default {
  name: "Skills",
  components: {
    Tile,
  },
  data: function () {
    return {
      phoneImg: phoneImg,
      bookImg: bookImg,
      desktopImg: desktopImg,
    };
  },
};
</script>

<style scoped>
#skills {
  width: 100%;
  margin-top: 12vh;
  padding: 0 7.5% 0 7.5%;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 75px;
  background-color: var(--secondary-background-color);
}

@media screen and (max-width: 750px) {
  #skills {
    grid-template-columns: 1fr;
  }
}
</style>
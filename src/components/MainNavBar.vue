<template>
  <div>
    <ul>
      <li><a href="#">Contact</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Skills</a></li>
      <li><a href="#">Work</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MainNavBar",
};
</script>

<style scoped>
* {
  background-color: rgba(0, 0, 0, 0);
}

div {
  margin-top: 2%;
}

ul {
  display: flex;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  list-style: none;
  justify-content: flex-end;
  text-align: center;
  margin-right: 2.5%;
}

li:first-child a {
  padding: 0px 10px 3px 10px;
  border-bottom: 2px solid var(--emphasised-color);
}

a {
  text-decoration: none;
  font-size: 115%;
  transition: font-size 0.5s, color 0.25s;
  margin: 20px;
}

a:hover {
  font-size: 125%;
  color: var(--emphasised-text-color);
}
</style>
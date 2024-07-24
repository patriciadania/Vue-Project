<template>
  <ul>
    <li><a href="#">HOME </a></li>
    <li><a href="#">PROJETO </a></li>
    <li><a href="#">CONTATOS</a></li>
  </ul>
</template>

<script>
export default {
  name: "Header",
};
</script>
<style scoped>
ul {
  list-style: none;
  display: flex;
  background-color: #999;
}
li {
  margin-right: 10px;
}
a {
  color: white;
  text-decoration: none;
  transition: 0.5s;
}
a:hover {
  color: turquoise;
}
</style>

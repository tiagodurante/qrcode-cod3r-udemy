<template>
  <div class="app">Hello World</div>
</template>

<script>
export default {};
</script>

<style>
@font-face {
  font-family: "Roboto";
  src: url("https://fonts.googleapis.com/css?family=Roboto&display=swap");
}
* {
  font-family: "Roboto", "monospace";
}
body {
  margin: 0;
}
#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff;
  background: linear-gradient(to right, rgb(83, 105, 118), rgb(41, 46, 73));
}
</style>
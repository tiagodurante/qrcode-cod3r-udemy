<template>
  <div id="app">
    <Main />
  </div>
</template>

<script>
import Main from "./main/Index";
export default {
  components: {
    Main
  }
};
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
.input {
  font-size: 2em;
  margin-bottom: 30px;
}
.output {
  border: 1px solid #222;
  padding: 30px 15px;
  background-color: #0006;
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
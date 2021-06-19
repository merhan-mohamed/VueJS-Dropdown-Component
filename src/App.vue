<template>
  <div id="app">
    <header>
      <Navbar />
    </header>
  </div>
</template>

<script type="text/javascript">
import Navbar from "./components/Navbar";
export default {
  name: "app",
  components: {
    Navbar,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: "montserrat", sans-serif;
}
header {
  width: 100%;
  background-color: #222;
  padding: 15px;
}
</style>

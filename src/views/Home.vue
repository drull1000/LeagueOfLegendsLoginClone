<template>
  <div id="app">
    <div class="container">
      <router-view />
      <Nickname />
      <Play />
      <Footer />
    </div>
  </div>
</template>

<script>
import Nickname from "../components/Nickname";
import Play from "../components/Play.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "App",
  components: {
    Nickname,
    Play,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@600;900&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  text-decoration: none;
  font-family: "Poppins", sans-serif;
}
.container {
  background: linear-gradient(rgba(22, 22, 22, 0.76), rgba(22, 22, 22, 0.76)),
    url("../assets/Login_image.jpg");
  background-size: cover;
  background-attachment: fixed;
  background-position: center;
  padding: 3.3rem;
}
</style>

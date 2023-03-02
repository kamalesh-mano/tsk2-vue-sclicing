<script>
 import navBar from "./components/navBar/navbar.vue";
 import bottom from "./components/Footer/footer.vue";
 import landingPage from "./components/landingPage/landingPage.vue"
 import Blog from "./components/Blog/Blog.vue"
 export default {
  components:{
    navBar,
    bottom,
    landingPage,
    Blog
  }
 }
</script>

<template>
  <div class="container">
    <navBar></navBar>
    <landingPage></landingPage>
    <Blog></Blog>
    <bottom></bottom>
  </div>
</template>

<style scoped>
.container{
  width: 1366px;
}
</style>

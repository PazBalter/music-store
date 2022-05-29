<template>
  <div class="home">
    <section class="hero">
      <div class="container">
      
      </div>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'HomePage',

}
</script>

<style lang="scss" scoped>
.hero{
  width: 100%;
  background-image:url("../assets/store-hero.jpg");
  background-position: center;
  background-repeat: no-repeat;
  position: relative;
  background-size:cover;
  height: 120vh;

  img{
    object-fit: cover;
    height: 100%;
    width: 100%;
  }

}
</style>
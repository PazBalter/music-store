<template>
  <div class="app">
    <appHeader/>
    <router-view/>
  </div>
</template>

<script>
import appHeader from "./cmps/app-header.vue";
export default{
  setup() {},
  components: {
    appHeader
  },
}
</script>

<style lang="scss">
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: sans-serif;
  font-weight: 400;
  
}

.app{
  //  height: 200vh;
  min-height: 100vh;
  // display: flex;
  position: relative;
  background-color: #f1f1f1;
}

.container{
  padding: 0 20px;
  max-width: 1140px;
  margin: 0 auto;
  
}

.flex-centered-column{
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.flex-row{
  display: flex;
  flex-direction: row;
 
}
</style>



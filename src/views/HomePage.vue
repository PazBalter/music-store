<template>
  <div class="home">
    <section class="hero">
      <div class="container">
        <div class="hero-text">
          <div class="hero-text-left">
            <div class="logo-box">
              <img src="@/assets/logo.png" alt="">
            </div>
            <router-link class="shop-link" :to="{ name: 'Shop' }"><div class="shop-button">SHOP NOW</div></router-link>
            <div class="slogan">
              Play Safe, Enjoy!
            </div>
          </div>
          <div class="hero-text-right">
            <h2> Join Us</h2>
            <div class="login-inputs">
              <input type="text">
              <input type="text">
            </div>
          </div>
        </div>
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
  height: 100vh;
  display: flex;
  

  img{
    object-fit: cover;
    height: 100%;
    width: 100%;
    
  }
  .hero-text{
    height: 100%;
    display: flex;
    // justify-content: center;
    align-items: center;
    flex-direction: row;
    // background-color: rgba(0, 0, 0, 0.6);
    color: #fff;
    gap: 10%;

    .hero-text-left{
      padding: 20px;
      border-radius: 10px;
       background-color: rgba(0, 0, 0, 0.6);
      width: 45%;
      // background: green;
      justify-content: center;

      .logo-box{
        padding: 0 40px;
      }
      .shop-link{
        text-decoration: none;

        .shop-button{
          text-align: center;
          padding: 10px;
          background: gold;
          border-radius: 4px;
          color: black;
          font-weight: 600;
          cursor: pointer;
          transition: 0.5s;
          &:hover{
            background: rgb(255, 108, 63);
          }
        }
      }
    }
    .hero-text-right{
      width: 45%;
      padding: 20px;
      border-radius: 10px;
      background-color: rgba(0, 0, 0, 0.6);
      text-align: center;

      h2{
        padding: 0;
        margin: 20px;
      }

      .login-inputs{
        display: flex; 
        flex-direction: column;
        

        input{
          padding: 5px;
        }
      }
    }
  }
}
</style>
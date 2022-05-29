<template>
  <header 
   :class="{ 'scrolled-nav' : scrollPosition }">
      <nav>
          <div class="header-logo">
              <img src="@/assets/logo.png" alt="">
          </div>
          <ul v-show="!mobile" class="navigation">
              <li><router-link class="link" :to="{ name: 'Shop' }">Shop</router-link></li>
              <!-- <li><router-link class="link" :to="{ name: '' }"></router-link></li> -->
              <li><router-link class="link" :to="{ name: 'About' }">Home</router-link></li>
              <li><router-link class="link" :to="{ name: 'Contact' }">Contact</router-link></li>
          </ul>
          <div class="hamburger-icon">
              <i @click="toggleMobileNav" v-show="mobile" :class="{'icon-active': mobileNav}"></i>
          </div>
          <transition name="mobile-nav"></transition>
          
      </nav>
  </header>
</template>
 <script>

 export default {
 data() {
    return {
      scrollPosition: true,
      mobile: false,
     
    };
  },
 }
 </script>
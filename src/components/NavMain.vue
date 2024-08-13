<template>
    <div class="navmain">
      <div class="desktop"> 
            <li>ABOUT</li>
            <li>CARREERS</li>
            <li>EVENTS</li>
            <li>PRODUCTS</li>
            <li>SUPPORT</li>
        </div>
      
    <img class="hamburger" src="../assets/images/icon-hamburger.svg" @click="isOpen = !isOpen" />
    <Slide :isOpen="isOpen" @closeMenu="isOpen = false">
      <img class="mobile" src="../assets/images/logo.svg" width="100px" height="20px"/>
       <nav> 
            <li>ABOUT</li>
            <li>CARREERS</li>
            <li>EVENTS</li>
            <li>PRODUCTS</li>
            <li>SUPPORT</li>
        </nav>
    </Slide>
  </div>
</template>

<script>

import { Slide } from 'vue3-burger-menu';

export default {
  components: {
    Slide
  },
  data() {
    return {
      isOpen: false
    };
  }
};

</script>

<style>
.bm-burger-button{
        display: none;
    }
  @media (max-width: 768px) {
    .bm-menu{
      width: 480px;
      background: black;
      font-family:'Alata' ;
      font-weight: 200;
    }
    .bm-menu li{
      padding-right: 5em;
    }
    .bm-menu span{
      margin-top: 2em;
      margin-right: 2em;
    }
  }
</style>
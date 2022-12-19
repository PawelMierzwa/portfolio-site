<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Nav from './components/Nav.vue'
</script>

<template>
  <header id="hmain">
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <Nav />
      <HelloWorld msg="TITLE :)" />
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
#hmain {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  #hmain {
    margin-top: 6%;
    display: flex;
    place-items: right;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  #hmain .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
  main{
    margin: 5% 5% 0 0;

  }
}
</style>

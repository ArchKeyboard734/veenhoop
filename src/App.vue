<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Hoofdmenu from './components/hoofdmenu.vue';
import gebruiker from './components/gebruiker.vue';
</script>

<template>

  <header>
    <!-- header goes here. full width of screen -->
    <!--import header out of the menubalkDocent-->
    <div class="hoofdmenu">
      <Hoofdmenu></Hoofdmenu>'
    </div>

    <div class="gebruiker">
      <gebruiker></gebruiker>
    </div>
  </header>
  <div class="main">

    <RouterView />
  </div>


  <!-- een div links en een div rechts -->
</template>

<style scoped>
/* .box {
  background-color: red;
  width: 100px;
  height: 100px;
} */

header {
  line-height: 1.5;
  max-height: 100vh;
  background-color: rgb(17, 0, 255);
  width: auto;
  height: auto;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
    background-color: red;
    width: 100px;
    height: 10px;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>

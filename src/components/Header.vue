<script>
import { headerMenu } from "../menues";
export default {
  computed: {
    mainMenu() {
      return headerMenu.main;
    },
    iconsMenu() {
      return headerMenu.icons;
    },
  },
};
</script>

<template>
  <header>
    <nav class="top">
      <!-- Categories -->
      <ul>
        <li v-for="(item, index) in mainMenu" :key="`m-${item}`">
          <a :href="item.href">{{ item.text }}</a>
        </li>
      </ul>

      <!-- Logo -->
      <img class="logo" src="/src/assets/img/boolean-logo.png" alt="logo" />

      <!-- Icons -->
      <div class="icons">
        <ul>
          <li v-for="(item, index) in iconsMenu" :key="`m-${item}`">
            <a :href="item.href">{{ item.text }}</a>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<style lang="scss">
@use "../assets/scss/main.scss";
</style>

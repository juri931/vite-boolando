<script>
export default {
  data() {
    return {
      menu: [
        {
          title: "Home",
          link: "#",
        },
        {
          title: "Chi siamo",
          link: "#",
        },
        {
          title: "Prodotti",
          link: "#",
        },
        {
          title: "Contatti",
          link: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <ul class="nav">
      <li class="nav-item" v-for="(item, index) in menu" :key="index">
        <a class="nav-link" aria-current="page" :href="item.link">{{
          item.title
        }}</a>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped></style>

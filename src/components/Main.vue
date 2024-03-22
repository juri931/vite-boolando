<script>
import { cards } from "../cards";

export default {
  computed: {
    cards() {
      return cards.main;
    },
  },
};
</script>

<template>
  <main>
    <div class="container">
      <div class="product" v-for="(item, index) in cards" :key="`m-${item}`">
        <img class="primary-img" :src="item.img" />
        <img class="img-hover" :src="item.imgHover" />
        <div class="disc-eco">
          <span class="discount">{{ item.discount }}</span>
          <span class="eco">{{ item.eco }}</span>
        </div>
        <span class="heart">{{ item.heart }}</span>

        <div class="info">
          <span class="brand">{{ item.brand }}</span>
          <span class="desc">{{ item.desc }}</span>
          <span class="price-new">{{ item.priceNew }}</span>
          <span class="price-old">{{ item.priceOld }}</span>
        </div>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use "../assets/scss/main.scss";

div {
  margin: 50% auto;
}
</style>

<script>
import { cards } from "../cards";

export default {
  computed: {
    cards() {
      return cards.main;
    },
  },
};
console.log(cards.main);
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
        <a :href="item.href">{{ item.text }}</a>

        <!-- <img class="primary-img" src="../assets/img/1.webp" alt="" />
        <img class="img-hover" src="../assets/img/1b.webp" alt="" />
        <div class="disc-eco">
          <span class="discount">-50% </span>
          <span class="eco">Sostenibilità</span>
        </div>
        <span class="heart">&hearts;</span>

        <div class="info">
          <span class="brand">Levi's</span>
          <span class="desc">relaxed fit tee unisex</span>
          <span class="price-new">14,99€</span>
          <span class="price-old">29,99€</span>
        </div>
      </div>

      <div class="product">
        <img class="primary-img" src="../assets/img/2.webp" alt="" />
        <img class="img-hover" src="../assets/img/2b.webp" alt="" />
        <div class="disc-eco">
          <span class="discount">-30%</span>
        </div>
        <span class="heart">&hearts;</span>
        <div class="info">
          <span class="brand">Guess</span>
          <span class="desc">roses tee</span>
          <span class="price-new">20,99€</span>
          <span class="price-old">29,99€</span>
        </div>
      </div>

      <div class="product">
        <img class="primary-img" src="../assets/img/3.webp" alt="" />
        <img class="img-hover" src="../assets/img/3b.webp" alt="" />
        <div class="disc-eco">
          <span class="discount">-30%</span>
        </div>
        <span class="heart">&hearts;</span>
        <div class="info">
          <span class="brand">Come Zucchero Filato</span>
          <span class="desc">voglia di colori pastello</span>
          <span class="price-new">129,99€</span>
          <span class="price-old">184,99€</span>
        </div>
      </div>

      <div class="product">
        <img class="primary-img" src="../assets/img/4.webp" alt="" />
        <img class="img-hover" src="../assets/img/4b.webp" alt="" />
        <div class="disc-eco">
          <span class="discount">-50%</span>
          <span class="eco">Sostenibilità</span>
        </div>
        <span class="heart">&hearts;</span>
        <div class="info">
          <span class="brand">Levi's</span>
          <span class="desc">tee unisex</span>
          <span class="price-new">14,99€</span>
          <span class="price-old">29,99€</span>
        </div>
      </div>

      <div class="product">
        <img class="primary-img" src="../assets/img/5.webp" alt="" />
        <img class="img-hover" src="../assets/img/5b.webp" alt="" />
        <div>
          <span class="heart">&hearts;</span>
        </div>
        <div class="info">
          <span class="brand">Maya Deluxe</span>
          <span class="desc">stripe bodice</span>
          <span class="price-new">99,99€</span>
        </div>
      </div>

      <div class="product">
        <img class="primary-img" src="../assets/img/6.webp" alt="" />
        <img class="img-hover" src="../assets/img/6b.webp" alt="" />
        <div class="disc-eco">
          <span class="eco">Sostenibilità</span>
        </div>
        <span class="heart">&hearts;</span>

        <div class="info">
          <span class="brand">Come Zucchero Filato</span>
          <span class="desc">voglia di colori pastello</span>
          <span class="price-new">129,99€</span>
          <span class="price-old">184,99€</span>
        </div> -->
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

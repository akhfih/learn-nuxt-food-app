<template>
  <nav>
    <ul>
      <li>
        <nuxt-link exact to="/"><AppLogo /></nuxt-link>
      </li>
      <li><nuxt-link exact to="/restaurants">Restaurants</nuxt-link></li>
      <li><nuxt-link exact to="/about">About</nuxt-link></li>
    </ul>
    <div class="smallnum" v-if="cartCount > 0">{{ cartCount }}</div>
    <nuxt-link exact to="/cart">Cart</nuxt-link>
  </nav>
</template>

<script>
import { mapGetters } from "vuex";
export default {
  computed: {
    ...mapGetters(["cartCount"]),
  },
};
</script>

<style lang="scss" scoped></style>

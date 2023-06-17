<template>
  <main class="container">
    <AppRestaurantInfo />
  </main>
</template>

<script>
import AppHeader from "../components/AppHeader.vue";
import AppRestaurantInfo from "../components/AppRestaurantInfo.vue";

export default {
  name: "IndexPage",
  components: { AppHeader, AppRestaurantInfo },
};
</script>

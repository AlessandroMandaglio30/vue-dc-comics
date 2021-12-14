<template>
  <main>
    <Hero />
  </main>
</template>

<script>
import Hero from "../components/Hero.vue";
export default {
  name: "Main",
  components: {
    Hero,
  },
};
</script>

<style scoped lang="scss">
main {
  background-color: #1c1c1c;
}
</style>
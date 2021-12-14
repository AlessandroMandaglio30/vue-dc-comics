<template>
  <main>
    <Hero />
    <Comics />
  </main>
</template>

<script>
import Hero from "../components/Hero.vue";
import Comics from "../components/Comics.vue";

export default {
  name: "Main",
  components: {
    Hero,
    Comics,
  },
};
</script>

<style scoped lang="scss">
main {
  background-color: #1c1c1c;
}
</style>
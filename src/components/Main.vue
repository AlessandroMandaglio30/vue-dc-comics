<template>
  <div class="main">
    <div class="main-cont">--&gt; Content goes here &lt;--</div>
  </div>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/partials/variables.scss";
.main {
  height: 150px;
  background-color: #1c1c1c;
  .main-cont {
    width: 80%;
    margin: 0 auto;
    font-size: 22px;
    color: #fff;
    padding: 60px 0;
  }
}
</style> 
<template>
  <header>
    <div class="header-cont">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="Logo-DC" />
        <nav>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">Tv</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Collectibles</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">Fans</a></li>
            <li><a href="#">News</a></li>
            <li><a href="#">Shop</a></li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  name: "Header",
};
</script>
<style lang="scss" scoped>
@import "../assets/style/partials/variables.scss";
header {
  margin-top: 20px;
  text-align: center;
  display: flex;
  margin-bottom: 20px;
}
.header-cont {
  width: 80%;
  margin: 0 auto;
}
.logo {
  margin-left: 50px;
  display: flex;
  img {
    height: 70px;
  }
}
nav {
  margin-top: 10px;
  // nav ul {}
  ul {
    margin-left: 60%;
    display: flex;
    justify-content: center;
    list-style: none;
    // nav ul li
    li a {
      text-transform: uppercase;
      font-weight: 500;
      font-size: 18px;
      display: inline-block;
      padding: 15px 20px;
      text-decoration: none;
      color: #000;
      // nav ul li a.active, nav ul li a:hover
      &.active,
      &:hover {
        background-color: $headerColor;
      }
    }
  }
}
</style>
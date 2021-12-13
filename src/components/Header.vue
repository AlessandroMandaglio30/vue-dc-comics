<template>
  <header>
    <div class="header-cont">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="Logo-DC" />
        <nav>
          <ul>
            <li
              v-for="(link, i) in links"
              :key="i"
              :class="link.visible ? 'active' : ''"
            >
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          visible: false,
        },
        {
          text: "COMICS",
          url: "#",
          visible: true,
        },
        {
          text: "MOVIES",
          url: "#",
          visible: false,
        },
        {
          text: "TV",
          url: "#",
          visible: false,
        },
        {
          text: "GAMES",
          url: "#",
          visible: false,
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          visible: false,
        },
        {
          text: "VIDEOS",
          url: "#",
          visible: false,
        },
        {
          text: "FANS",
          url: "#",
          visible: false,
        },
        {
          text: "NEWS",
          url: "#",
          visible: false,
        },
        {
          text: "SHOP",
          url: "#",
          visible: false,
        },
      ],
    };
  },
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
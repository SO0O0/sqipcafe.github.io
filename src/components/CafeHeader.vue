<template>
  <header class="header">
    <div class="container">
      <div class="inner">
        <div class="title">
          <h1 class="logo">
            <a href="#">
              <img src="../assets/logo.png" alt="SQIP Cafe" />
            </a>
            <p class="intro" v-if="windowWidth > 1100">新横浜のスペシャルティコーヒー専門店</p>
          </h1>
        </div>
        <div class="menu" v-if="windowWidth > 850">
          <ul class="info">
            <li>
              <a href="#">アクセス</a>
            </li>
            <li>
              <a href="#">サイトマップ</a>
            </li>
            <li class="iquiry">
              <a href="#">お問い合わせ</a>
            </li>
          </ul>
          <nav class="global_menu">
            <ul>
              <li>
                <a href="#">HOME</a>
              </li>
              <li>
                <a href="#">CONCEPT</a>
              </li>
              <li>
                <a href="#">DRINK</a>
              </li>
              <li>
                <a href="#">CAKE</a>
              </li>
              <li>
                <a href="#">FOOD</a>
              </li>
              <li>
                <a href="#">TAKEOUT</a>
              </li>
            </ul>
          </nav>
        </div>
        <div class="humberger" v-if="windowWidth < 849">
          <HumbergerMenu />
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import HumbergerMenu from "./Humberger.vue";

export default {
  name: "CafeHeader",
  components: {
    HumbergerMenu
  },
  data() {
    return {
      windowWidth: "10000",
      menuOpen: ""
    };
  },
  mounted() {
    window.addEventListener("resize", this.resizeWindow);
  },
  methods: {
    resizeWindow() {
      this.windowWidth = window.innerWidth;
    }
  }
};
</script>

<style lang="scss" scoped>
.header {
  width: 100%;
  position: absolute;
  z-index: 100;

  h1 {
    font-size: 12px;
    display: flex;
    height: auto;
    align-items: center;
  }

  .container {
    .inner {
      display: flex;
      justify-content: space-between;

      .title {
        color: #fff;
        margin-top: 20px;
        margin-left: 3%;

        img {
          font-size: 0;
          margin-right: 10px;
          vertical-align: top;
        }
      }

      .info {
        color: #fff;
        margin-left: auto;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        font-weight: normal;
        width: 100%;
        font-size: 13px;

        li {
          list-style: none;
          padding-top: 10px;
          margin-left: 5%;
        }

        .iquiry {
          background: #f4bb00;
          padding: 15px 40px;

          a {
            color: #000;
            font-weight: bold;
          }
        }
      }

      .global_menu {
        margin-top: 5%;
        ul {
          width: 50%;
          display: flex;
          font-size: 16px;

          li {
            margin-right: 50px;
            list-style: none;
            font-weight: bold;
          }
        }
      }
    }
  }
}
</style>

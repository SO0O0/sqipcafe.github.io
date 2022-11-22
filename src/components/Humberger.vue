<template>
  <div>
    <!--ハンバーガーメニューのボタン-->
    <div class="hamburger-btn" @click="active=!active">
      <span class="line line-top" :class="{'rotate-top':active}"></span>
      <span class="line line-middle" :class="{'rotate-middle':active}"></span>
      <span class="line line-bottom" :class="{'rotate-bottom':active}"></span>

      <!--ハンバーガーメニューの中身-->
      <transition name="hamburger-menu">
        <div class="hamburger-menu" v-show="active">
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

          <ul class="info">
            <li>
              <a href="#">アクセス</a>
            </li>
            <li>
              <a href="#">サイトマップ</a>
            </li>
            <li>
              <a href="#">お問い合わせ</a>
            </li>
          </ul>
        </div>
      </transition>
    </div>
  </div>
</template>

<script>
export default {
  name: "HumbergerMenu",
  data() {
    return {
      active: false
    };
  }
};
</script>

<style scoped>
/* ハンバーガーメニューのボタンのcss */
.hamburger-btn {
  position: fixed;
  top: 10.5px;
  left: 85%;
  width: 70px;
  height: 72px;
  cursor: pointer;
  z-index: 50;
}
.line {
  position: absolute;
  top: 0;
  left: 20px;
  width: 45px;
  height: 2px;
  background: #eee;
  text-align: center;
}
.line-top {
  top: 16px;
  transition: 0.4s ease;
}
.line-middle {
  top: 26px;
  transition: 0.4s ease;
}
.line-bottom {
  top: 36px;
  transition: 0.4s ease;
}
.rotate-top {
  transform: translateY(10px) rotate(-45deg);
  transition: 0.4s ease;
}
.rotate-middle {
  transition: 0.4s ease;
  opacity: 0;
}
.rotate-bottom {
  transform: translateY(-10px) rotate(45deg);
  transition: 0.4s ease;
}

/* ハンバーガーメニューの中身のcss */
.hamburger-menu-enter-active,
.hamburger-menu-leave-active {
  opacity: 0.4;
}
.hamburger-menu-enter,
.hamburger-menu-leave-to {
  opacity: 0;
}
.hamburger-menu-leave,
.hamburger-menu-enter-to {
  opacity: 1;
}
.hamburger-menu {
  background-color: #222;
  z-index: 30;
  padding: 2rem 1rem;
  position: fixed;
  width: 300px;
  height: 80rem;
  top: 0;
  right: 0;
}
ul {
  padding: 0;
  padding-top: 40px;
}
li {
  padding: 5% 0;
  list-style: none;
  line-height: 1;
}
a {
  color: #eee;
  text-decoration: none;
  font-size: 1.1;
  margin: 0 4vw;
}
</style>

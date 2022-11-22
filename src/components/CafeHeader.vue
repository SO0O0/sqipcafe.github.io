<template>
  <header class="header">
    <div class="container">
      <div class="inner">
        <div class="title">
          <h1 class="logo">
            <a href="#">
              <img src="../assets/logo.png" alt="SQIP Cafe" />
            </a>
            <p class="time">新横浜のスペシャルティコーヒー専門店</p>
          </h1>
        </div>
        <div class="menu">
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
      </div>
      <div class="hamburger">
        <span></span>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "CafeHeader"
};
</script>

<style lang="scss" scoped>
.header {
  display: block;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 100;
  opacity: 1;

  h1 {
    font-size: 12px;
    display: flex;
    height: auto;
    align-items: center;
  }

  .container {
    margin: 0 auto;
    width: 100%;

    .inner {
      display: flex;
      justify-content: space-between;

      .title {
        text-align: center;
        color: #fff;
        font-weight: 700;
        line-height: 150%;
        margin-top: 20px;

        .logo {
          margin-bottom: 5px;

          img {
            line-height: 1;
            font-size: 0;
            height: auto;
            max-width: 100%;
            margin-right: 10px;
            vertical-align: top;
          }
        }
      }

      .info {
        color: #fff;
        margin-left: auto;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        font-weight: 700;
        width: 380px;
        border-radius: 0 0 10px 10px;
        margin-bottom: 20px;
        font-size: 13px;

        li {
          list-style: none;
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
        ul {
          display: flex;
          font-size: 16px;

          li {
            margin-right: 50px;
            list-style: none;
          }
        }
      }
    }
  }
}
</style>

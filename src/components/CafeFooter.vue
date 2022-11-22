<template>
  <footer class="footer">
    <div class="container">
      <p class="logo">
        <a href="#">
          <img src="../assets/logo_2.png" alt="SQIP Cafe" />
        </a>
      </p>
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
    <div class="bottom">
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
      <p class="copyright">&copy;&nbsp;SQIP Inc. All rights reserved.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "CafeFooter"
};
</script>

<style lang="scss" scoped>
.footer {
  height: auto;
  background: #291e15;

  .container {
    margin: 0 auto;
    width: 80%;
    .logo {
      text-align: center;
      padding: 43px 0;
    }

    .global_menu {
      width: 50%;
      margin: 0 auto;
      ul {
        display: flex;
        justify-content: space-between;
        font-size: 16px;

        li {
          font-weight: bold;
          list-style: none;
        }
      }

      @media screen and (max-width: 768px) {
        ul {
            display: block;
            li {
                text-align: center;
                margin-bottom: 10px;
            }
        }
      }
    }
  }

  .bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-top: 1px solid rgba(254, 254, 254, 0.3);
    margin-top: 70px;
    padding-top: 35px;

    .info {
      margin-left: 45px;
      display: flex;
      align-items: center;
      justify-content: flex-start;
      width: 380px;
      border-radius: 0 0 10px 10px;
      margin-bottom: 35px;
      font-size: 13px;

      li {
        list-style: none;
        margin-right: 25px;
      }
    }

    .copyright {
      color: #fff;
      font-size: 11px;
      margin: 0 45px 35px 0;
    }

    @media screen and (max-width: 768px) {
        flex-direction: column;
        align-items: center;
        justify-content: center;

        li {
            width: 100%;
        }

        .copyright {
            margin:0 0 35px 0;
        }
    }
  }
}
</style>

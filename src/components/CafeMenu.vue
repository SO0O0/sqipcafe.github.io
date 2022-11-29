<template>
  <div class="container">
    <div class="headline">
      <h2>MENU</h2>
      <p>
        SQIP Cafeは新鮮な食材で丁寧に仕上げた料理を
        <br />お客様にお届けしています。
      </p>
    </div>
    <ul class="list">
      <li class="box">
        <img src="../assets/drink.png" alt="DRINK" />
        <h3>
          <span class="en">DRINK</span>
          <span class="ja">ドリンク</span>
        </h3>
        <p class="descri">本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります</p>
      </li>
      <li class="box">
        <img src="../assets/cake.png" alt="DRINK" />
        <h3>
          <span class="en">CAKE</span>
          <span class="ja">ケーキ</span>
        </h3>
        <p class="descri">本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります</p>
      </li>
      <li class="box">
        <img src="../assets/food.png" alt="FOOD" />
        <h3>
          <span class="en">FOOD</span>
          <span class="ja">フード</span>
        </h3>
        <p class="descri">本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります</p>
      </li>
    </ul>
    <p class="detail">
      <a href="#">詳しくはこちら</a>
    </p>
  </div>
</template>

<script>
export default {
  name: "CafeMenu"
};
</script>

<style lang="scss" scoped>
.container {
  height: auto;
  width: 80%;
  margin: 0 auto;
  .headline {
    text-align: center;

    h2 {
      font: normal normal 900 44px/24px Nato Sans JP;
      padding-top: 60px;
      margin-bottom: 5%;
    }

    p {
      color: #666;
    }
  }

  .list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    margin-top: 60px;
    list-style: none;

    @media screen and (min-width: 769px) {
      li:nth-child(2) {
        margin: 0 1rem;
      }
    }
    p {
      color: #666;
    }

    .box {
      width: 30%;

      @media screen and (max-width: 768px) {
        width: 80%;
        margin: 3% auto;
      }

      img {
        width: 100%;
      }

      h3 {
        .en {
          font-size: 30px;
          display: block;
          margin-bottom: 1%;
        }

        .ja {
          font-size: 12px;
          display: block;
          color: #f4bb00;
          margin-top: -0.5em;
          margin-bottom: 3%;
        }
      }
    }
  }

  .detail {
    text-align: center;
    padding-bottom: 90px;

    a {
      display: inline-block;
      color: #000;
      background: #f4bb00;
      font-size: 14px;
      text-align: center;
      max-width: 220px;
      width: 100%;
      padding: 18px 0;
      margin-top: 40px;
    }
  }
}
</style>

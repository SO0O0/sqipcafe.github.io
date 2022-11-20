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
        <div>
          <img src="../assets/drink.png" alt="DRINK" />
        </div>
        <h3>
          <span class="en">DRINK</span>
          <span class="ja">ドリンク</span>
        </h3>
        <p class="descri">本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります</p>
      </li>
      <li class="box">
        <div>
          <img src="../assets/drink.png" alt="DRINK" />
        </div>
        <h3>
          <span class="en">CAKE</span>
          <span class="ja">ケーキ</span>
        </h3>
        <p class="descri">本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります本文が入ります</p>
      </li>
      <li class="box">
        <div>
          <img src="../assets/food.png" alt="FOOD" />
        </div>
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
  height: 100vh;
  max-width: 1100px;
  margin: 0 auto;
  .headline {
    text-align: center;

    h2 {
      padding-top: 60px;
    }

    p {
      color: #666;
    }
  }

  .list {
    display: flex;
    justify-content: space-between;
    margin-top: 60px;

    li:nth-child(2) {
      margin: 0 1rem;
    }

    .box {
      width: 30%;

      h3 {
        .en {
          font-size: 30px;
          display: block;
        }

        .ja {
          font-size: 12px;
          display: block;
          color: #f4bb00;
          margin-top: -0.5em;
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

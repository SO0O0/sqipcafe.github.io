<template>
  <article class="bnr">
    <ul class="container">
      <li>
        <a href="#">
          <img src="../assets/bnr_1.png" alt="SQIP:BtoBの企業サイト専門web制作会社" />
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/bnr_2.png" alt="画像を入れてください" />
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/bnr_2.png" alt="画像を入れてください" />
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/bnr_2.png" alt="画像を入れてください" />
        </a>
      </li>
    </ul>
  </article>
</template>

<script>
export default {
  name: "CafeBanner"
};
</script>

<style lang="scss" scoped>
article {
    background: #faf8f7;

    ul {
        display: flex;
        justify-content: center;

        li {
            margin: 50px 17px;
            list-style: none;
        }
    }
}
</style>

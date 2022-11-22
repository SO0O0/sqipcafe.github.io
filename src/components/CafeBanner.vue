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

    @media screen and (max-width: 768px) {
        .container {
            display: block;

            li {
                padding: 3%;
                margin: 0 auto;
                width: 50%;
            }
        }
    }

    ul {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;

        li {
            margin: 5% 1%;
            width: 18%;
            list-style: none;

            img {
                width: 100%;
            }
        }
    }
}
</style>

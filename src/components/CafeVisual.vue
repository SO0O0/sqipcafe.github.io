<template>
  <div class="mv">
    <div class="inner">
      <p class="label">
        しあわせを
        <br />感じるひとときを
      </p>
      <p class="guide">新鮮なコーヒー豆「香りのカプセル」をお届けします．</p>
      <p class="more">
        <a href="#">MORE</a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "CafeVisual"
};
</script>

<style lang="scss" scoped>
.mv {
  height: 100vh;
  background-image: url("../assets/main_visual.png");
  background-size: cover;
  position: relative;
  z-index: 1;

  .inner {
    position: absolute;
    top: 30%;
    left: 50%;
    transform: translate(-50%, 0);
    text-align: center;
    width: 100%;
    z-index: 2;

    .label {
      font-size: 5vw;
      color: #fff;
      letter-spacing: 5px;
      font-weight: lighter;

      @media screen and (max-width: 768px) {
        font-size: 8vw;
      }
    }

    .guide {
      color: #fff;
      margin-top: 2%;
    }

    .more {
      margin-top: 4%;

      a {
        display: inline-block;
        padding: 1% 0;
        color: #f4bb00;
        border: 1px solid #f4bb00;
        width: 15%;
        font-size: 14px;
        text-decoration: none;
      }
    }
  }
}
</style>

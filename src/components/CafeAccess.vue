<template>
  <div class="access">
    <div class="container">
      <div class="headline">
        <h2>
          <span class="en">ACCESS</span>
        </h2>
        <address>〒222-0033 神奈川県横浜市港北区新横浜2-12-12 新横浜IKビル304</address>
      </div>
      <div class="information_map">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3247.806797707558!2d139.6107088156088!3d35.50905524700201!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60185ed391eb65b5%3A0x9fcc0f0c3ce88635!2z44CSMjIyLTAwMzMg56We5aWI5bed55yM5qiq5rWc5biC5riv5YyX5Yy65paw5qiq5rWc77yS5LiB55uu77yR77yS4oiS77yR77ySIOaWsOaoqua1nO-8qe-8q-ODk-ODqw!5e0!3m2!1sja!2sjp!4v1614088176897!5m2!1sja!2sjp"
          allowfullscreen
          loading="lazy"
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CafeAccess"
};
</script>

<style lang="scss" scoped>
.access {
  .container {
    margin: 0 auto;
    width: 100%;

    h2 {
      font: normal normal 900 44px/24px Nato Sans JP;
      text-transform: uppercase;
      padding-top: 60px;
      margin-bottom: 3%;
    }

    .headline {
      text-align: center;

      address {
        font-style: normal;
        color: #666;
        margin: 8px 0 60px;
      }
    }

    .information_map {
      height: 0;
      overflow: hidden;
      padding-bottom: 80vh;
      position: relative;

      iframe {
        position: absolute;
        left: 0;
        top: 0;
        border: 0;
        height: 100%;
        width: 100%;
      }
    }
  }
}
</style>

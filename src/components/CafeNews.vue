<template>
  <div class="news">
    <div class="container">
      <div class="head_line">
        <h2>NEWS</h2>
      </div>
      <div class="info">
        <div class="list">
          <p class="date">2019.10.11</p>
          <p class="emergency">緊急のお知らせ</p>
          <p class="txt">明日12日（土）は台風19号のため終日休業とさせていただきます。ご了承ください。</p>
        </div>
        <div class="list">
          <p class="date">2019.09.12</p>
          <p class="new">新メニュー</p>
          <p class="txt">コーヒー豆が新しくなりました。</p>
        </div>
        <div class="list">
          <p class="date">2019.09.01</p>
          <p class="new">新メニュー</p>
          <p class="txt">期間限定！マロンケーキが新登場。まろやかなマロンクリームと新鮮な生クリームの組み合わせが絶品です。</p>
        </div>
        <div class="list">
          <p class="date">2019.08.25</p>
          <p class="info">お知らせ</p>
          <p class="txt">公式サイトをリニューアルしました。</p>
        </div>
      </div>
      <p class="detail">
        <a href="#">詳しくはこちら</a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "CafeNews"
};
</script>

<style lang="scss" scoped>
.news {
  width: 100%;
  background: #f8f6f5;
  .container {
    background: #f8f6f5;
    margin: 0 auto;
    padding-left: 15px;
    padding-right: 15px;
    width: 80%;

    .head_line {
      text-align: center;

      h2 {
        padding-top: 60px;

        .en {
          font-size: 44px;
        }
      }

      p {
        color: #666;
      }
    }

    .info {
      text-align: center;
      margin: 40px auto 0;

      .list {
        display: flex;
        line-height: 2em;
        color: #666;
        margin: 1.5em 0;

        .emergency {
          min-width: 120px;
          max-height: 2em;
          background: #de1212;
          border-radius: 0.3em;
          color: #fff;
          text-align: center;
          margin: 0 1.2em;
        }

        .new {
          min-width: 120px;
          max-height: 2em;
          background: #849c64;
          border-radius: 0.3em;
          color: #fff;
          text-align: center;
          margin: 0 1.2em;
        }

        .info {
          min-width: 120px;
          max-height: 2em;
          background: #6e94b4;
          border-radius: 0.3em;
          color: #fff;
          text-align: center;
          margin: 0 1.2em;
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
}
</style>

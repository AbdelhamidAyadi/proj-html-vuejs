<template>
  <div class="aboutme_container">
    <div class="section_title">ABOUT ME</div>

    <div class="description_container">
      <div class="title">
        How to Be an Alpha Male: The 15 Habits of True Alphas
      </div>
      <div class="description">
        <div>
          Want to learn how to be <span>an alpha male</span> ? How to be more masculine? How to be the man you've always
          wanted to be?
        </div>
        <div>
          Your goal is to show the consistency of business, core values, and customer care. Punctuality, responsibility,
          individuality, accuracy, enthusiasm - you have to clearly explain how these qualities are applicable to your
          work. And the important thing is you do love what you do.
        </div>
      </div>
    </div>

    <div class="video_container">
      <div class="video">
        <img class="video_thumbnail" src="../assets/img/home-movation-video-poster-670x450.jpg" alt="">
        <img class="youtube_logo" src="../assets/img/icon-youtube-play.png" alt="">
      </div>
      <div class="quote_container">
        <div class="quote">
          "Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."
        </div>
        <div class="credits">
          <img src="../assets/img/home-movation-shape-01.png" alt="">
          <div>Kaixa Stark</div>
          <div>WINGMAN</div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
  export default {
    name: 'AboutMeComp',

  }
</script>

<style scoped lang="scss">
  .aboutme_container {
    padding: 0 15%;
    margin: 100px 0;

    .section_title {
      color: #20ad96;
      font-weight: bold;
      margin-bottom: 20px;
    }

    .description_container {
      display: flex;
      margin-bottom: 50px;

      .title {
        width: 50%;
        font-size: 2rem;
        padding-right: 20%;
        font-weight: 600;
      }

      .description {
        width: 50%;

        div:first-of-type {
          font-weight: 600;
          margin-bottom: 20px;

          span {
            color: #20ad96;
          }
        }

        div:nth-of-type(2) {
          font-size: 0.9rem;
          color: rgb(116, 116, 116);
        }
      }
    }

    .video_container {
      display: flex;
      align-items: center;
      margin: 50px 0;

      .video {
        display: inline-block;
        width: 55%;
        position: relative;

        .video_thumbnail {
          border-radius: 10px;
          filter: brightness(70%);
          height: 100%;
          width: 100%;
        }

        .youtube_logo {
          position: absolute;
          right: 50%;
          top: 50%;
          bottom: 50%;
          left: 50%;
          transform: translate(-50%, -50%);


        }

      }
      .quote_container{
        width: 45%;
        padding-left:100px;
        .quote{
          font-size: 2rem;
          line-height: 3rem;
          font-weight: lighter;
          margin-bottom: 50px;
        }
        .credits{
          > * {
            padding-bottom: 10px;
          }
          div:first-of-type{
            font-weight: bolder;
            font-size: 1.2rem;
          }
          div:nth-of-type(2){
            color: grey;
          }
        }
      }

    }

  }
</style>
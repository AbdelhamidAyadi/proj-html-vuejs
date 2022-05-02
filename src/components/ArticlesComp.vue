<template>
  <div class="articles_container">
    <div class="title">
      <div>BLOG UPDATED</div>
      <div>Interesting <span>articles updated</span> daily</div>
    </div>
    <div class="articles">

      <div v-for="(element , index) in articles" :key="index" class="article">
        <div class="image">
          <img :src="element.image" alt="">
        </div>
        <div class="date">
          <i class="fa-regular fa-calendar"></i>
          {{element.date}}
        </div>
        <div class="title">
          {{element.title}}
        </div>
        <div class="description">
          {{element.title}}
        </div>
      </div>
    </div>
    <div class="more_articles">
      <a href="#" >
      VIEW ALL POSTS
      </a>
    </div>



  </div>
</template>

<script>
  export default {
    name: 'ArticlesComp',
    data() {
      return {
        articles: [{
            title: "How to Stay True to your Personal Brand",
            image: require('../assets/img/motivation-blog-04-480x325.jpg'),
            date: "May 13,2020",
            description: "When it comes to your business or career, you want ...",
          },
          {
            title: "5 Vital Lessons in 5 Years of Freelancing",
            image: require('../assets/img/motivation-blog-03-480x325.jpg'),
            date: "May 13,2020",
            description: "Being self-employed and working from home, it's easy to get ...",
          },
          {
            title: "11 Super Useful Tips for Small Business Owners",
            image: require('../assets/img/motivation-blog-02-480x325.jpg'),
            date: "May 13,2020",
            description: "Being a small-business owner poses a ton of challenges. We...",
          },
          {
            title: "How to Give Yourself Grace to Start Again",
            image: require('../assets/img/motivation-blog-01-480x325.jpg'),
            date: "May 13,2020",
            description: "Forgive yourself for bad habits you may have started or ...",
          }
        ]
      }
    }
  }
</script>

<style scoped lang="scss">
  .articles_container {
    margin: 100px 0;
    padding: 0 15%;
  }

  .title {
    margin: 50px 10px;
    div:first-of-type {
      color: grey;
      font-weight: 600;
    }

    div:nth-of-type(2) {
      font-size: 2.5rem;
      margin: 15px 0;

      span {
        color: #20ad96;
      }
    }
  }

  .articles {
    display: flex;
    flex-wrap: wrap;
  }

  .article {
    width: 25%;
    padding: 0 10px;

    .image img {
      height: 100%;
      width: 100%;
      border-radius: 10px;
    }

    .date {
      color: gray;
      font-size: 0.8rem;
      margin: 15px 0;

      i {
        padding-right: 5px
      }
    }

    .title {
      font-size: 1.1rem;
      font-weight: bold;
      line-height: 1.8rem;
      color: black;
      margin: 15px 0;
    }

    .description {
      color: gray;
      font-size: 0.9rem;
    }
  }
  .more_articles{
    margin: 50px 0;
    
    text-align: center;
    a{
      color: #20ad96;
    }
  }
</style>
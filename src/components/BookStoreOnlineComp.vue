<template>
  <div class="bookStoreOnline_container">
    <div class="books_description">
      <div class="description">
        <div>
          BOOK STORE ONLINE
        </div>
        <div>
          <span>Be Alpha With </span>
          <span>Wingmans's Book</span>
        </div>
      </div>
      <div class="books_benefits">
        <ul>
          <li><i class="fa-solid fa-check"></i> Help you understand yourself better</li>
          <li><i class="fa-solid fa-check"></i> Revealing mature tips</li>
          <li><i class="fa-solid fa-check"></i> Give the right advice</li>
          <li><i class="fa-solid fa-check"></i> Fascinating examples of alpha man</li>
        </ul>
      </div>
      <button>
        Get Free EBook

      </button>
    </div>
    <div class="books_container">
      <div v-for="(element , index) in books" :key="index" class="book">
        <div class="book_cover">
          <img :src="element.image">
          <div class="options">
            <div>
              <i class="fa-solid fa-magnifying-glass"></i>
            </div>
            <div>
              <i class="fa-solid fa-cart-shopping"></i>
            </div>
           <div>
              <i class="fa-solid fa-heart"></i>
           </div>
           <div>
              <i class="fa-solid fa-signal"></i>
           </div>
          </div>
        </div>
        <div class="book_details">
          <div>{{element.name}}</div>
          <div><span>${{element.priceDollars}}</span><span>{{element.priceCents}}</span></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'BookStoreOnlineComp',
    data() {
      return {
        books: [{
            name: "Alpha man by Maxcoach",
            image: require('../assets/img/product-book-11-400x400.jpg'),
            priceDollars: "29",
            priceCents: ".00"
          },
          {
            name: "Real man 4.0 by Maxcoach",
            image: require('../assets/img/product-book-10-400x400.jpg'),
            priceDollars: "39",
            priceCents: ".00"
          }
        ]
      }
    }

  }
</script>

<style scoped lang="scss">
  .bookStoreOnline_container {
    padding: 0 15%;
    margin: 100px 0;
    display: flex;
  }

  .description {
    div:first-of-type {
      font-weight: 600;
      color: gray;
    }

    div:nth-of-type(2) {
      font-size: 2.5rem;
      margin: 30px 0;

      span:first-of-type {
        color: #413c65;

      }

      span:nth-of-type(2) {
        color: #20ad96;
      }
    }
  }

  .books_description {
    width: 40%;
  }

  .books_benefits {
    ul {
      list-style: none;
      line-height: 2rem;
      margin: 30px 0;

      li {
        i {
          color: #20ad96;
          margin-right: 15px;
        }

        font-size: 0.9rem;
        font-weight: 600;
        color: rgb(143, 142, 142);
      }
    }
  }

  button {
    padding: 15px 40px;
    border-radius: 10px;
    border-color: #20ad96;
    background: #20ad96;
    color: white;
    font-weight: bold;

    &:hover {

      background: #3f3a64;
      border-color: #3f3a64;
      cursor: pointer;
    }

  }

  .books_container {
    width: 60%;
    display: flex;

  }

  .book {
    width: 50%;
    padding: 0 10px;

    .book_cover {
      position: relative;
      img {
        height: 100%;
        width: 100%;
      }
      .options{
        position: absolute;
        right: 10px;
        top: 10px;
        i{
          padding: 7px;
          margin: 2px 0;
          background: rgb(227, 225, 225);
          border-radius: 50% ;
          cursor: pointer;
          display: none;
          

        }

      }
      &:hover i{
        display: inline-block;
      }

    }

    >* {
      padding-bottom: 15px;
    }

    .book_details {
      text-align: center;

      div:first-of-type {
        font-size: 1.1rem;
        font-weight: bold;
        line-height: 2rem;
        color: #362d79;
      }

      div:nth-of-type(2) {
        color: #20ad96;
        font-weight: bold;

        span:first-of-type {
          font-size: 1.5rem;

        }
      }

    }




  }
</style>
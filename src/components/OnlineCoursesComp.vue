<template>
  <div class="onlineCourses_container">
    <div class="title_container">
      <div>BEGIN YOUR JOURNEY AT MAXCOACH</div>
      <div>Latest <span>Online Courses</span></div>
    </div>
    <div class="courses_container">
      <div v-for="( element , index ) in courses" :key="index" class="course">
        <div>
          <img :src="element.image" :alt="element.name + 'thumbnail'">
        </div>
        <div class="course_details">
          <div>
            <span>${{element.priceDollars}}</span>{{element.priceCents}}
          </div>
          <div>
            {{element.name}}
          </div>
          <div>
            <span><i class="fa-regular fa-file-lines"></i>{{element.lessons}} Lessons</span>
            <span><i class="fa-regular fa-user"></i>{{element.students}} Students</span>
          </div>
        </div>
      </div>
    </div>
    <div>
      <button>
        View all courses
        <i class="fa-solid fa-right-long"></i>
      </button>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'OnlineCoursesComp',
    props: {},
    data() {
      return {
        courses: [{
            name: "How to be Successful: Create A Growth Mindset For Success",
            image: require('../assets/img/motivation-course-06-480x298.jpg'),
            priceDollars: "30",
            priceCents: ".00",
            lessons: "3",
            students: "50"
          },
          {
            name: "How to Build Confidence in Your Abilities",
            image: require('../assets/img/motivation-course-05-480x298.jpg'),
            priceDollars: "30",
            priceCents: ".00",
            lessons: "1",
            students: "50"
          },
          {
            name: " Productivity Machine - Focus in a Distracted World",
            image: require('../assets/img/motivation-course-04-480x298.jpg'),
            priceDollars: "20",
            priceCents: ".00",
            lessons: "10",
            students: "50"
          },
          {
            name: "Effective Time Management Mastery - Complete Guide",
            image: require('../assets/img/motivation-course-03-480x298.jpg'),
            priceDollars: "20",
            priceCents: ".00",
            lessons: "18",
            students: "50"
          },
          {
            name: "Body Language Secrets for Entrepreneurs",
            image: require('../assets/img/motivation-course-02-480x298.jpg'),
            priceDollars: "25",
            priceCents: ".99",
            lessons: "19",
            students: "50"
          },
          {
            name: "Management Skills: The Science of Leadership",
            image: require('../assets/img/motivation-course-01-480x298.jpg'),
            priceDollars: "19",
            priceCents: ".99",
            lessons: "17",
            students: "50"
          }

        ]
      }
    }
  }
</script>

<style scoped lang="scss">
  .onlineCourses_container {
    padding: 0 15%;
    margin: 100px 0;
    text-align: center;
  }

  .title_container {
    margin-bottom: 50px;

    div:first-of-type {
      color: grey;
      font-weight: 600;
    }

    div:nth-of-type(2) {
      font-size: 3rem;
      font-weight: 600;

      span {
        color: #20ad96;
      }
    }
  }

  .courses_container {
    display: flex;
    flex-wrap: wrap;


    .course {
      width: calc(100%/3);
      padding: 0 10px;
      padding-bottom: 20px;

      img {
        width: 100%;
        height: 100%;
        border-radius: 10px;
      }

      .course_details {
        >* {
          padding-bottom: 15px;
        }

        div:first-of-type {
          color: #20ad96;
          font-weight: bold;

          span:first-of-type {
            font-size: 2rem;

          }
        }

        div:nth-of-type(2) {
          font-size: 1.1rem;
          font-weight: bold;
          line-height: 2rem;
          color: #362d79;
        }

        div:nth-of-type(3) {
          color: gray;
          font-size: 0.8rem;

          span {
            padding-right: 20px;

            i {
              padding-right: 5px
            }
          }
        }

        padding: 20px;
        text-align: left;
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

      background: #2ab7a0b0;
      ;
    }

  }
</style>
<template>
  <div class="realStoriesContainer">
    <div class="left_side">
      <p>REAL STORIES</p>
      <p>I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the
        syllabus. Great study portal for people like me.</p>
      <div>
        <img src="../assets/img/testimonial-avata-02.jpg" alt="">
      </div>
      <p>Mina Hollace</p>
      <p>/ Freelancer</p>
    </div>
    <div class="right_side">
      <img src="../assets/img/home-movation-testimonial-image.jpg" alt="">
    </div>
    <div class="switcher">
      <div>
        <img src="../assets/img/image.png" >
      </div>
      <p>1/4</p>
      <div>
        <img src="../assets/img/image (1).png">
      </div>
    </div>

  </div>
</template>

<script>
  export default {
    name: 'RealStoriesComp',
    props: {}
  }
</script>

<style scoped lang="scss">
  .realStoriesContainer {
    display: flex;
    position: relative;

  }

  .left_side {
    width: 50%;
    background-image: url('../assets/img/background-pattern-wavify.png');
    background-color: #f7f7fd;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 0 10%;
    img{
      height: 100px;
      width: 100px;
      border-radius: 50%;
      margin-bottom: 30px;
    }
    p:first-of-type{
      color: #20ad96;
      font-weight: bold;
      margin-bottom: 30px;
    }
    p:nth-of-type(2){
      font-size: 1.5rem;
      font-weight: 350;
      margin-bottom: 30px;
    }
    p:nth-of-type(3){
      color:grey;
      font-weight: bold;
      margin-bottom: 30px;
    }
    p:nth-of-type(4){
      color:grey;
      font-size: 0.8rem;
      margin-bottom: 30px;
    }
  }

  .right_side {
    width: 50%;

    img {
      width: 100%;
      height: 100%;

    }
  }
  .switcher{
    position: absolute;
    top: 50%;
    bottom: 50%;
    right: 50%;
    left: 50%;
    transform: translate(-50% , -50%);
    height: 70px;
    width: 70px;
    display: flex;
    flex-direction: column;
    border-radius: 50%;
    background: white;
    justify-content: center;
    align-items: center;

  }
</style>
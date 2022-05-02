<template>
  <div class="footer_container">
    <div class="informations">
      <div class="adress">
        <div class="title">Address</div>
        <ul>
          <li>382 NE 191st St # 87394 Miami, FL 33179-3899</li>
          <li>+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)</li>
          <li>support@maxcoach.com</li>
          <li class="social_container">
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-facebook"></i>
            <i class="fa-brands fa-instagram"></i>
            <i class="fa-brands fa-linkedin-in"></i>
          </li>
        </ul>
      </div>
      <div class="explore_and_information">
        <div class="explore">
          <div class="title">Explore</div>
          <div>
            <div>
              <ul>
                <li>Start here</li>
                <li>Blog</li>
                <li>About us</li>
              </ul>
            </div>
            <div>
              <ul>
                <li>Success story</li>
                <li>Courses</li>
                <li>Contact us</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="information">
          <div class="title">Information</div>
          <div>
            <div>
              <ul>
                <li>Membership</li>
                <li>Purchase guide</li>
                <li>Privacy policy</li>
                <li>Terms of service</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="copyrights">
      © 2020 Maxcoach. All Rights Reserved
    </div>
  </div>
</template>

<script>
  export default {
    name: 'footerComp',
    props: {}
  }
</script>

<style scoped lang="scss">
  .footer_container {
    padding: 50px 15%;
    font-size: 0.8rem;
    line-height: 2rem;
    background-color: #171621;
    color: rgb(184, 181, 181);
    i{
      margin-right: 15px;
      font-size: 1rem;
    }
    .informations{
      
      display: flex;
      ul{
        list-style: none;
        
      }
     
    }
    .explore{

      div:nth-of-type(2){
        display: flex;
        div{
          margin-right:50px;
        }
      }
    }
    .explore_and_information{
      width: 50%;
      display: flex;
    }
    .adress{
      width: 50%;
    }
  }
  .title{
    color: white;
    font-size: 1rem;
    font-weight: 600;
  }
  .copyrights{
    text-align: center;
    margin-top: 50px ;
  }
</style>
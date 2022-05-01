<template>
  <div class="container_nav">
    <div class="logo_container"><img src="../assets/img/dark-logo.png" alt=""></div>
    <div class="menu_container">
      <ul>
        <li v-for="(element , index) in menu" :key="index">
          {{element}}
          <i class="fa-solid fa-angle-down"></i>
        </li>
      </ul>
    </div>
    <div class="social_container">
      <i class="fa-brands fa-twitter"></i>
      <i class="fa-brands fa-facebook"></i>
      <i class="fa-brands fa-instagram"></i>
      <i class="fa-brands fa-linkedin-in"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavComp',
  props: {
  },
  data(){
    return{
      menu:["Home","Pages","Courses","Features","Blog","Shop"]
    }
  }
}
</script>

<style scoped lang="scss">
.container_nav{
  display: flex;
  padding: 20px 15%;
  justify-content: space-between;
}
.logo_container{
  img{
    width: 100%;
    height: 100%;
  }
  width: 15%;
}
.menu_container{
  ul {
    list-style: none;
    display: flex;
    li{
      padding: 0 15px;
      display: flex;
      align-items: center;
      i{
        padding: 0 5px;
      }

    }
  }
}
.social_container{
  display: flex;
  justify-content: space-around;
  width: 15%;
}
</style>

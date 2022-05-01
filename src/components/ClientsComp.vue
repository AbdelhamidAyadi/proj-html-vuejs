<template>
  <div class="sponsors_container">
    <img src="../assets/img/client-logo-05-primary.png">
    <img src="../assets/img/client-logo-06-primary.png">
    <img src="../assets/img/client-logo-07-primary.png">
    <img src="../assets/img/client-logo-04-primary.png">
    <img src="../assets/img/client-logo-03-primary.png">
    <img src="../assets/img/client-logo-02-primary.png">
  </div>
</template>

<script>
export default {
  name: 'ClientsComp',
  props: {
  }
}
</script>

<style scoped lang="scss">
.sponsors_container{
  padding: 0 15%;
  margin: 100px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  img{
    height: 100%;
    filter: grayscale(100%) opacity(30%);
  }
}

</style>

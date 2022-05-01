<template>
  <div>
    <header>
      <NavComp/>
      <HomePageComp/>
    </header>
    <main>
      <StatisticsComp/>
    </main>
  </div>
</template>

<script>
import NavComp from './components/NavComp.vue'
import HomePageComp from './components/HomePageComp.vue'
import StatisticsComp from './components/StatisticsComp.vue'

export default {
  name: 'App',
  components: {
    NavComp,
    HomePageComp,
    StatisticsComp
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
header{
  background-image: url('./assets/img/background-pattern-wavify.png');
}
</style>

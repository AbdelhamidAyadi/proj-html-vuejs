<template>
  <div>
    <header>
      <NavComp/>
      <HomePageComp/>
    </header>
    <main>
      <StatisticsComp/>
      <AboutMeComp/>
      <OnlineCoursesComp/>
      <BookStoreOnlineComp/>
      <ClientsComp/>
      <RealStoriesComp/>
    </main>
  </div>
</template>

<script>
import NavComp from './components/NavComp.vue'
import HomePageComp from './components/HomePageComp.vue'
import StatisticsComp from './components/StatisticsComp.vue'
import AboutMeComp from './components/AboutMeComp.vue'
import OnlineCoursesComp from './components/OnlineCoursesComp.vue'
import BookStoreOnlineComp from './components/BookStoreOnlineComp.vue'
import ClientsComp from './components/ClientsComp.vue'
import RealStoriesComp from './components/RealStoriesComp.vue'

export default {
  name: 'App',
  components: {
    NavComp,
    HomePageComp,
    StatisticsComp,
    AboutMeComp,
    OnlineCoursesComp,
    BookStoreOnlineComp,
    ClientsComp,
    RealStoriesComp,
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
  background-color: #f7f7fd;
}
</style>

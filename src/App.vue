<template>
  <div id="app">
    <Header />
    <main>
      <section></section>
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header'
export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style lang="scss">
  @import '@/style/global';
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500&display=swap');
  *{
    font-family: 'Roboto', sans-serif;
  }
  #app{
    height: 100vh;
  }
  main{
    height: 40%;
    section:first-child{
        height: 50%;
        width: 100% ;
        background-color:black ;
    }

  }
  

</style>

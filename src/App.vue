<template>
  <div id="app">
    <Header />
    <main>
      <section></section>
      <OptionSection/>
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header'
import OptionSection from '@/components/OptionSection'
export default {
  name: 'App',
  components: {
    Header,
    OptionSection,
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
    height: 50%;
    section:first-child{
        height: 40%;
        width: 100% ;
        background-color:black ;
    }

  }
  

</style>

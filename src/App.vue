<template>
  <div id="app">
    <Header />
    <main>
      <section class="container"><h2>-->Content goes here</h2></section>
      <OptionSection/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header'
import OptionSection from '@/components/OptionSection'
import Footer from '@/components/Footer'
export default {
  name: 'App',
  components: {
    Header,
    OptionSection,
    Footer,
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
    display: flex;
    flex-direction: column;
    }
  main{
    height: 40%;
    section:first-child{
        height: 40%;
        width: 100% ;
        background-color:black ;
        h2{
          color: white;
        }
    }

  }
  

</style>

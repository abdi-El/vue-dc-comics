<template>
  <div id="app">
    <Header />
    <main>
      <Hero />
      <OptionSection/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header'
import OptionSection from '@/components/OptionSection'
import Hero from '@/components/Hero'
import Footer from '@/components/Footer'
export default {
  name: 'App',
  components: {
    Header,
    OptionSection,
    Footer,
    Hero,
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
    main{
      background-color: #1c1c1c;
    }
    }
</style>

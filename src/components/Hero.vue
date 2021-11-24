<template>
  <section>
      <div class="hero"></div>
      <div class="comics container">
          <div>
              <button>CURRENT SERIES</button>
          </div>
          <ul>
              <Comics v-for='(comic, index) in comics' :key='`comic-${index}`' :comicName='comic.series' :imgPath='comic.thumb'/>
          </ul>
      </div>
  </section>
</template>

<script>
import comics from '@/data/dc-comics.js'
import Comics from '@/components/Comics.vue'
export default {
    name: 'Hero',
    data(){
        return{
            comics,
        }
    },
    components:{
        Comics
    }
}
</script>

<style lang='scss' scoped>
    @import '@/style/utilities';
    section{
        color: white;
        background-color:#1c1c1c ;
        .hero{
            height: 400px;
            background-image: url('../assets/jumbotron.jpg');
            background-size: cover;
        }
        .comics{
            padding: 0px 25px ;
            position: relative;
            top: -25px;
            button{
                color: white;
                font-size: 16px;
                font-weight: 600;
                background-color: dodgerblue;
                padding: 15px 20px;
                border: none;
            }
            ul{
                width: 100%;
                margin: 20px 0px;
                display: flex;
                flex-wrap: wrap;
            }
        }
    }
</style>
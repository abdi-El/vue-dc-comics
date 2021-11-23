<template>
  <header>
      <div class="container">
        <img src="@/assets/dc-logo.png" alt="">
        <ul>
            <li v-for='(link, index) in links' :key="`link-${index}`">
                <h3>{{link.text}}</h3>
            </li>
        </ul>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return{
            links : [
                {
                    text: 'CHARACTERS',
                    active: false, 
                },
                {
                    text: 'COMICS',
                    active: true, 
                },
                {
                    text: 'MOVIES',
                    active: false, 
                },
                {
                    text: 'TV',
                    active: false, 
                },
                {
                    text: 'GAMES',
                    active: false, 
                },
                {
                    text: 'COLLECTIBLES',
                    active: false, 
                },
                {
                    text: 'VIDEOS',
                    active: false, 
                },
                {
                    text: 'FANS',
                    active: false, 
                },
                {
                    text: 'NEWS',
                    active: false, 
                },
                {
                    text: 'SHOP',
                    active: false, 
                },
            ]
        
        }
    }
}
</script>

<style scoped>
    .container{
        height: 100px;
    }
</style>
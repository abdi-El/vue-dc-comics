<template>
  <header class="display-flex">
      <div class="container display-flex">
        <img src="@/assets/dc-logo.png" alt="">
        <ul class="display-flex">
            <li v-for='(link, index) in this.links' :key='`link-${index}`' :class={active:link.active}>
                <span>{{link.text}}</span>
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

<style scoped lang='scss'>
    @import '@/style/utilities';
    header{
        height: 20%;
    }
    .container{
        justify-content: space-between;
        align-items: center;
        li{
            margin: 10px;
            line-height: 100px;
            font-size: 14px;
            color: #464646;
            &:hover{
                border-bottom:5px solid dodgerblue;
                color: dodgerblue !important;
                cursor: pointer;
            }
        }
    }
    .active{
        border-bottom:5px solid dodgerblue;
        color: dodgerblue !important;
    }
    
</style>
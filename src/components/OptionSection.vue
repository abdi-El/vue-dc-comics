<template>
    <section class="display-flex">
        <div class="display-flex container">
            <div v-for="(obj, index) in this.objects" :key='`obj-${index}`' class="option-container">
                <img :src='require(`../assets/${obj.img}`)' :alt="obj.text">
                <span>{{obj.text}}</span>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'OptionSection',
    data(){
        return{
            objects:[
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    img: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: 'buy-dc-power-visa.svg',
                    text: 'DC MERCHANDISE'
                }
            ]
        }
    }
}
</script>

<style lang='scss' scoped>
    @import '@/style/utilities';
    section{
        background-color: dodgerblue;
        height: 200px;
        div{
            align-items: center;
            padding: 15px;
            .option-container{
                display: flex;
                align-items: center;
                width: 20%;
                height: 100%;
                color: white;
                font-size: 13px;
                font-weight: 300;
                img{
                    width: 30%;
                }
                span{
                    margin: 0 5px
                }
            }
        }
    }
</style>
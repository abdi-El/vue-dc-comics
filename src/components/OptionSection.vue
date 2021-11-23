<template>
    <section class="display-flex container">
        <div v-for="(obj, index) in this.objects" :key='`obj-${index}`'>
            <img :src="obj.img" :alt="obj.text">
            <span>{{obj.text}}</span>
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
                    img: '@/assets/dc-logo.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    img: '@/assets/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    img: '@/assets/buy-comics-subsriptions.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    img: '@/assets/buy-comics-shop--locator.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: '@/assets/buy-dc-power-visa.svg',
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
        justify-content: space-between;
        div{
            font-size: 14px;
        }
    }
</style>
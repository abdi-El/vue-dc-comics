<template>
    <li>
        <img :src="imgPath" :alt="comicName">
        <span>{{comicName}}</span>
    </li>
</template>

<script>
export default {
    name: 'comics',
    props:{
        comicName: String,
        imgPath: String
    }
}
</script>

<style scoped lang='scss'>
    li{
        list-style: none;
        width: calc(100%/6);
        padding: 8px;
        margin-bottom:20px ;
        img{
            width: 100%;
            object-fit: cover;
            transition: scale 0.3s;
            &:hover{
                scale: 1.05;
                cursor: pointer;
            }
        }
        span{
            display: inline-block;
            margin-top: 10px;
        }
    }
</style>
<script>
export default {
    props:{
        myComic: Object,
    }
}
</script>

<template >
    <div class="comics">
        <img :src="myComic.thumb">
        <p>{{ myComic.series }}</p>
    </div>
</template>

<style lang="scss" scoped>
    img{
        width: 180px;
        margin-top: 50px;
        aspect-ratio: 1/1;
        object-fit: cover;
        object-position: center;
    }
    p{
        font-size: 13px;
        text-transform: uppercase;
    }
   
</style>
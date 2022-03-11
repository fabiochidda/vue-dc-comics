<template>

    <div class="comic-card">
        <figure class="comic-image">
            <img :src="imgSrc" alt="">
        </figure>

        <div class="comic-title">
            <h3>{{comicTitle}}</h3>
        </div>

    </div>

</template>

<script>
export default {
    name: 'MsComic',
    props: {
        imgSrc: {
            type: String,
            required: true
        },
        comicTitle: {
            type: String,
            required: true
        }
    }
}
</script>

<style lang="scss" scoped>

.comic-card {
    width: calc(100% / 6);
    margin-bottom: 20px;

    .comic-image {
        aspect-ratio: 1/1;
        overflow: hidden;
        
        img {
            display: block;
        }
    }
}

.comic-title {

    h3 {
        margin-top: 15px;
        text-transform: uppercase;
        color: white;
    }
}

</style>
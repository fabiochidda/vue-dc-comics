<template>

    <section>
        <div class="container">
            <div class="container-lg">
                <ul class="merch-container">
                    <li v-for="(el, i) in merch" :key="i">
                        <img :src="el.imgSrc" alt="">
                        <p>{{el.text}}</p>
                    </li>
                </ul>
            </div>
        </div>
    </section>
    
</template>

<script>
export default {
    name: 'MsMerchandise',
    data () {
        return {
            merch: [
                {
                    text: 'DIGITAL COMICS',
                    imgSrc: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    text: 'DC MERCHANDISE',
                    imgSrc: require('../assets/img/buy-comics-merchandise.png')
                },
                {
                    text: 'SUBSCRIPTION',
                    imgSrc: require('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    imgSrc: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    text: 'DC POWER VISA',
                    imgSrc: require('@/assets/img/buy-dc-power-visa.svg')
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.container {
    background-color: #0282F9;
}

.container-lg {
    padding: 60px 30px;
}

.merch-container {
    width: 100%;
    display: flex;
    justify-content: space-between;

    li {
        display: flex;
        gap: 15px;
        align-items: center;

        p {
            color: white;
        }
    }
}

img {
    display: block;
    height: 40px;
}

</style>
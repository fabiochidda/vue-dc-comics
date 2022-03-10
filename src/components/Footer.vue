<template>
    <footer>
        <section>
            <div class="container footer">
                <div class="container-lg">
                    <div class="list-container">
                        <div class="col">
                            <ul>
                                <li class="list-title">
                                    <h2>{{listTitleGeneral}}</h2>
                                </li>
                                <li v-for="(el,i) in listGeneral" :key="i">
                                    <a href="#">{{el.text}}</a>
                                </li>
                            </ul>
                            <ul>
                                <li class="list-title">
                                    <h2>{{listTitleShop}}</h2>
                                </li>
                                <li v-for="(el,i) in listShop" :key="i">
                                    <a href="#">{{el.text}}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li class="list-title">
                                    <h2>{{listTitleDcTerms}}</h2>
                                </li>
                                <li v-for="(el,i) in listDcTerms" :key="i">
                                    <a href="#">{{el.text}}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li class="list-title">
                                    <h2>{{listTitleSites}}</h2>
                                </li>
                                <li v-for="(el,i) in listSites" :key="i">
                                    <a href="#">{{el.text}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section>
            <div class="container social-bar">
                <div class="container-lg">
                    <div class="sign">
                        <button>SIGN-UP NOW!</button>
                    </div>
                    <div class="social-links">
                        <p>FOLLOW US</p>
                        <ul class="social-list">
                            <li v-for="(el, i) in social" :key="i">
                                <img :src="el.imgSrc" alt="">
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'MsFooter',
    data () {
        return {
            listTitleGeneral: 'DC COMICS',
            listTitleShop: 'SHOP',
            listTitleDcTerms: 'DC',
            listTitleSites: 'SITES',
            listGeneral: [
                {
                    text: 'Characters'
                },
                {
                    text: 'Comics'
                },
                {
                    text: 'Movies'
                },
                {
                    text: 'TV'
                },
                {
                    text: 'Games'
                },
                {
                    text: 'Videos'
                },
                {
                    text: 'News'
                },
            ],
            listShop: [
                {
                    text: 'Shop DC'
                },
                {
                    text: 'Shop DC Collectibles'
                },
            ],
            listDcTerms: [
                {
                    text: 'Terms Of Use'
                },
                {
                    text: 'Privacy policy (New)'
                },
                {
                    text: 'Ad Choices'
                },
                {
                    text: 'Advertising'
                },
                {
                    text: 'Jobs'
                },
                {
                    text: 'Subscriptions'
                },
                {
                    text: 'Talent Workshops'
                },
                {
                    text: 'CPSC Certificates'
                },
                {
                    text: 'Ratings'
                },
                {
                    text: 'Shop Help'
                },
                {
                    text: 'Contact Us'
                },
            ],
            listSites: [
                {
                    text: 'DC'
                },
                {
                    text: 'MAD Magazine'
                },
                {
                    text: 'DC Kids'
                },
                {
                    text: 'DC Universe'
                },
                {
                    text: 'DC Power Visa'
                },
            ],
            social: [
                {
                    imgSrc: require('../assets/img/footer-facebook.png')
                },
                {
                    imgSrc: require('../assets/img/footer-twitter.png')
                },
                {
                    imgSrc: require('../assets/img/footer-youtube.png')
                },
                {
                    imgSrc: require('../assets/img/footer-pinterest.png')
                },
                {
                    imgSrc: require('../assets/img/footer-periscope.png')
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.container.footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: 100%;
    background-repeat: no-repeat;
}

.col {
    width: calc(100% / 9);
    padding-bottom: 5px;
}

.list-container {
    display: flex;
    flex-grow: 1;
    gap: 15px;
    padding: 60px 0;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
    background-size: 50%;

    li {
        padding-bottom: 10px;
    }

    h2 {
        color: white;
        padding-bottom: 10px;
    }

    a {
        color: #647177;
    }
}

.container.social-bar {
    background-color: #303030;
}

.social-bar .container-lg {
    justify-content: space-between;
}

.sign {
    align-self: center;
    button {
        padding: 15px;
        color: white;
        background-color: #303030;
        border: 2px solid #0183FB;;
    }
}

.social-links {
    display: flex;
    padding: 30px 0;
    align-items: center;

    p {
        color: #0183FB;
        font-size: 18px;
        font-weight: bold;
        margin-right: 20px;
    }
}

.social-list {
    display: flex;
    gap: 15px;
}
</style>
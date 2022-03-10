<template>
    <footer>
        <div class="container">
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
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.container {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: 100%;
    background-repeat: no-repeat;
    padding: 60px 0;
}

.col {
    width: calc(100% / 9);
    padding-bottom: 5px;
}

.list-container {
    display: flex;
    flex-grow: 1;
    gap: 15px;

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
</style>
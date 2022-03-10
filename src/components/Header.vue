<template>
    <header>
        <div class="container">
            <div class="container-lg">
                <figure class="header-logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </figure>
                <nav class="nav-container">
                    <ul class="nav">
                        <li v-for="(el, i) in navLinks" :key="i" class="nav-links" :class=" navLinks[i].isActive ? 'active' : '' ">
                            <a :href="el.href">{{el.text}}</a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'MsHeader',
    data() {
        return {
            navLinks: [
                {
                    text: 'CHARACTERS',
                    href: '#',
                    isActive: true,
                },
                {
                    text: 'COMICS',
                    href: '#',
                },
                {
                    text: 'MOVIES',
                    href: '#'
                },
                {
                    text: 'TV',
                    href: '#'
                },
                {
                    text: 'GAMES',
                    href: '#'
                },
                {
                    text: 'COLLECTIBLES',
                    href: '#'
                },
                {
                    text: 'VIDEOS',
                    href: '#'
                },
                {
                    text: 'FANS',
                    href: '#'
                },
                {
                    text: 'NEWS',
                    href: '#'
                },
                {
                    text: 'SHOP',
                    href: '#'
                }, 
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.container-lg{
    min-height: 130px;
    justify-content: space-between;
}

.header-logo {
    align-self: center;
}

.nav-container {
    display: flex;
    gap: 25px;
}

.nav {
    display: contents;
}

.nav-links {

    a {
        display: flex;
        align-items: center;
        height: 100%;
        font-size: 15px;
        font-weight: bold;
        position: relative;
    }

    &.active {
        a::after {
            content: '';
            display: block;
            height: 5px;
            position: absolute;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: #0282F9;
        }
    }

}



</style>
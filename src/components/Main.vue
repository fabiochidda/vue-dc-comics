<template>
    <main>
        <Jumbotron />

        <section>

        </section>

        <Merchandise />
    </main>
</template>

<script>
import Jumbotron from '../components/Jumbotron.vue'
import Merchandise from '../components/Merchandise.vue'

export default {
    name: 'MsMain',
    components: {
        Jumbotron,
        Merchandise
    }
}
</script>

<style lang="scss" scoped>



</style>
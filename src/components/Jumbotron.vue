<template>

    <section>
        <div class="container ms_jumbo">
            <div class="container-lg">
                <div class="current_series">
                    <p>CURRENT SERIES</p>
                </div>               
            </div>
        </div>
    </section>

</template>

<script>
export default {
    name: 'MsJumbotron'
}
</script>

<style lang="scss" scoped>

.container {
    background-image: url(../assets/img/jumbotron.jpg);
    background-position: top;
    min-height: 400px;
    background-size: 100%;
}

.container-lg {
    height: 400px;
    position: relative;
    align-items: flex-end;
}

.current_series {
    position: absolute;
    transform: translateY(50%);
    background-color: #0282F9;
    box-shadow: 5px 5px 5px black;

    p {
        color: white;
        padding: 20px;
    }

}

</style>
<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            listHeader: [
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop',
            ],
        }
    }
}
</script>

<template>
    <!-- Header -->
    <header class="py-2">
        <div class="container">
            <div class="row">
                <div class="col">
                    <div class="logo">
                        <img src="/img/dc-logo.png" alt="">
                    </div>
                </div>
                <div class="col d-flex align-items-center">
                    <ul class="d-flex">
                        <li class="mx-2" v-for="item in listHeader"> {{ item.toUpperCase() }}</li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>


<style lang="scss">
ul {
    list-style: none;
}
</style>
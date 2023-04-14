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
                <nav class="col d-flex align-items-center">
                    <ul class="d-flex mb-0 h-100 align-items-center">
                        <li class="mx-2 py-4" v-for="item in listHeader"> {{ item.toUpperCase() }}</li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>


<style lang="scss" scoped>
ul {
    list-style: none;

    li {
        cursor: pointer;
    }

    li:hover {
        border-bottom: 10px solid #0282f9;
        margin-top: 10px;
    }
}
</style>
<script>
    export default {
        data() {
            return {
                content: '--> Content goes here <--',
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
                ]
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
                        <li class="mx-2" v-for="item in listHeader"> {{item.toUpperCase()}}</li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
    <!-- Main -->
    <main>
        <div class="container">
            <div class="row">
                <div class="col">
                    <h2 class="text-white py-4">{{content}}</h2>
                </div>
            </div>
        </div>
    </main>

    <!-- Blue strip -->
    <section class="strip">
        <div class="container">
            <div class="row">
                <div class="col">
                    <ul>
                        <li>
                            <div class="picture">
                                <img src="" alt="">
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Info -->
    <section class="info">
        <div class="container">
            <div class="row">
                <div class="col">
                    <div class="dbl_list">
                        <ul></ul>
                        <ul></ul>
                    </div>
                    <ul></ul>
                    <ul></ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="row">
                <button class="sign_up">SIGN-UP NOW!</button>
                <div class="icon">
                    <span>FOLLOW US</span>
                </div>       
            </div>
        </div>
    </footer>
</template>

<style>
ul {
    list-style: none;
}

main {
    background-color: black;
}

.strip{
    background-color: #0282f9;
}
</style>

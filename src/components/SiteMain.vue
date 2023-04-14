<script>
import cards from '../data/data.js';
export default {
    name: 'SiteMain',
    data() {
        return {
            cards: cards
        }
    }

}
</script>

<template>
    <!-- Main -->
    <main>
        <div class="jumbotron">
            <img src="/img/jumbotron.jpg" alt="">
        </div>
        <div class="container">
            <div class="row">
                <div class="col">
                    <h2 class="text-white py-4">{{cards[0].series}}</h2>
                </div>
            </div>
        </div>
    </main>
</template>


<style lang="scss" scoped>
main {
    background-color: black;
}

.jumbotron {
    width:100%;
}

.jumbotron > img {
    max-width: 100%;
    width:100%;
    height: 350px;
    object-fit: cover;
    object-position: top;
}
</style>
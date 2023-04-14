<script>
import cards from '../data/data.js';
import JumboTron from './JumboTron.vue'
import CardThumb from './CardThumb.vue'
export default {
    name: 'SiteMain',
    components: {
        JumboTron,
        CardThumb
    },
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
        <JumboTron />
        <div class="container">
            <div class="row">
                <div class="col d-flex justify-content-between flex-wrap position-relative">
                    <div class="series text-uppercase text-white px-2 py-1 fw-bold fs-5">current series</div>
                    <CardThumb v-for="card in cards" :src="card.thumb" :title="card.series" />
                </div>
            </div>
            <button class="text-white text-uppercase mt-5 px-5 py-2 fw-bold">Load More</button>
        </div>
    </main>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
main {
    background-color: $darker;
    padding-bottom: 2rem;

    button {
        background-color: $blue-strip;
        display: block;
        margin: auto;
        border: 0;
    }
}
.series {
        position:absolute;
        top: -15px;
        left:0px;
        background-color: $blue-strip;
    }
</style>
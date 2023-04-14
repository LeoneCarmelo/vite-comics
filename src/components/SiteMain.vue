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
                <div class="col d-flex justify-content-between flex-wrap">
                    <CardThumb v-for="card in cards" :src="card.thumb" :title="card.series" />
                </div>
            </div>
        </div>
    </main>
</template>


<style lang="scss" scoped>
main {
    background-color: black;
}



</style>
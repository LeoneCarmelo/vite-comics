<script>
import cards from '../data/data.js';
import JumboTron from './JumboTron.vue'
export default {
    name: 'SiteMain',
    components: {
        JumboTron
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


</style>
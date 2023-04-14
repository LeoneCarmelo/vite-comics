<script>
export default {
    name: 'SiteMain',
    data() {
        return {
            content: '--> Content goes here <--'
        }
    }

}
</script>

<template>
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
</template>


<style lang="scss" scoped>
main {
    background-color: black;
}
</style>
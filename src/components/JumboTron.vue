<script>
export default {
    name: 'JumboTron'
}
</script>

<template>
        <div class="jumbotron">
            <img src="/img/jumbotron.jpg" alt="">
        </div>
</template>

<style lang="scss" scoped>
.jumbotron {
    width:100%;
    
    img {
       max-width: 100%;
       width:100%;
       height: 350px;
       object-fit: cover;
       object-position: top;
    }
}

</style>
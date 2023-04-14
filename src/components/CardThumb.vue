<script>
export default {
    name: 'CardThumb',
    props: {
        src: String,
        title: String
    }

}
</script>

<template>
    <div class="card_thumbs pt-5">
        <div class="thumb_body">
            <img :src="src" alt="">
        </div>
        <div class="thumb_head text-white pt-2">{{ title }}</div>
    </div>
</template>


<style lang="scss" scoped>
.thumb_body:hover {
    box-shadow: 0 0 2px 4px #0282f9;
}
.thumb_body {
    width:170px;
    height: 170px;

}

img {
    width: 100%;
    height: 170px;
    object-fit: cover;
    object-position: top;
    display: block;
}

.thumb_head {
    width: 170px;
    word-break: break-word;
}


</style>
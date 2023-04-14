<script>
import listStrip from '../data/sectionStrip.js'
export default {
    name: 'SectionStrip',
    data() {
        return {
            listStrip: listStrip
        }
    }

}
</script>
<template>
    <!--Section Blue strip -->
    <section class="strip py-3">
        <div class="container">
            <div class="row">
                <div class="col">
                    <ul class="d-flex align-items-center mb-0">
                        <li v-for="item in listStrip" class="d-flex mx-auto align-items-center">
                            <div class="picture">
                                <img :src="item.img" alt="">
                            </div>
                            <span class="text-white ms-2">{{ item.title.toUpperCase() }}</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
.strip{
    background-color: $blue-strip;
}

.picture {
    width:50px;

    img {
        max-width: 100%;
    }
}

ul li:nth-child(4)  img {
    height:60px;
}
</style>
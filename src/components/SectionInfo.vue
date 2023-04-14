<script>
import {dblList, shopList, dcList, sitesList} from '../data/sectionInfo.js'
export default {
    name: 'SectionInfo',
    data() {
        return {
            dblList: dblList,
            shopList: shopList,
            dcList: dcList,
            sitesList: sitesList
        }
    }

}
</script>
<template>
    <!-- Info -->
    <section class="info py-5">
        <div class="container">
            <div class="row">
                <div class="col d-flex">
                    <div class="dbl_list me-3">
                        <h3 class="text-white fw-bold">DC COMICS</h3>
                        <ul>
                            <li v-for="item in dblList"> {{ item }}</li>
                        </ul>
                        <h3 class="text-white fw-bold">SHOP</h3>
                        <ul>
                            <li v-for="item in shopList">{{ item }}</li>
                        </ul>
                    </div>
                    <div class="list_1 me-3">
                        <h3 class="text-white fw-bold">DC</h3>
                        <ul>
                            <li v-for="item in dcList">{{ item }}</li>
                        </ul>
                    </div>
                    <div class="list_2 me-3">
                        <h3 class="text-white fw-bold">SITES</h3>
                        <ul>
                            <li v-for="item in sitesList">{{ item }}</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
.info {
    background:  url('/img/dc-logo-bg.png') right  no-repeat, url('/img/footer-bg.jpg') center;

    ul {
        padding-left: 0;
        list-style: none;
    }

    li {
        color: $text-gray;
        cursor: pointer;
    }

    li:hover {
        color: $blue-strip;
    }
}
</style>
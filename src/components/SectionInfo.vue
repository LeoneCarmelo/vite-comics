<script>
export default {
    name: 'SectionInfo',
    data() {
        return {
            dblList: [
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News'
                ],
                shopList: [
                    'Shop DC',
                    'Shop DC Collectibles'
                ],
                dcList: [
                    'Terms Of Use',
                    'Privacy policy (New)',
                    'Ad Choices',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Workshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us',
                ],
                sitesList: [
                    'DC',
                    'MAD Magazine',
                    'DC Kids',
                    'DC Universe',
                    'DC Power Visa'
                ]
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
.info {
    background:  url('/img/dc-logo-bg.png') right  no-repeat, url('/img/footer-bg.jpg') center;

    ul {
        padding-left: 0;
        list-style: none;
    }

    li {
        color: #8c8b8b;
        cursor: pointer;
    }

    li:hover {
        color:#0282f9;
    }
}
</style>
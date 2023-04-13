<script>
    export default {
        data() {
            return {
                content: '--> Content goes here <--',
                listHeader: [
                    'characters',
                    'comics',
                    'movies',
                    'tv',
                    'games',
                    'collectibles',
                    'videos',
                    'fans',
                    'news',
                    'shop',
                ],
                listStrip: [
                    {
                        img: '/img/buy-comics-digital-comics.png',
                        title: 'digital comics'
                    },
                    {
                        img: '/img/buy-comics-merchandise.png',
                        title: 'dc merchandise'
                    },
                    {
                        img: '/img/buy-comics-subscriptions.png',
                        title: 'subscriptions'
                    },
                    {
                        img: '/img/buy-comics-shop-locator.png',
                        title: 'comic shop locator'
                    },
                    {
                        img: '/img/buy-dc-power-visa.svg',
                        title: 'dc power visa'
                    },
                ],
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
    <!-- Header -->
    <header class="py-2">
        <div class="container">
            <div class="row">
                <div class="col">
                    <div class="logo">
                        <img src="/img/dc-logo.png" alt="">
                    </div>
                </div>
                <div class="col d-flex align-items-center">
                    <ul class="d-flex">
                        <li class="mx-2" v-for="item in listHeader"> {{item.toUpperCase()}}</li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
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

    <!-- Blue strip -->
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

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="row">
                <button class="sign_up">SIGN-UP NOW!</button>
                <div class="icon">
                    <span>FOLLOW US</span>
                </div>       
            </div>
        </div>
    </footer>
</template>

<style>
ul {
    list-style: none;
}

main {
    background-color: black;
}

.strip{
    background-color: #0282f9;
}

.picture {
    width:50px;
}

.picture > img {
    max-width: 100%;
}

.info {
    background-image: url('/img/footer-bg.jpg');
}
.info ul {
    padding-left: 0;
}

.info li {
    color: #8c8b8b;
}

</style>

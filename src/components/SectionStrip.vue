<script>
export default {
    name: 'SectionStrip',
    data() {
        return {
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
        }
    }

}
</script>
<template>
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
.strip{
    background-color: #0282f9;
}

.picture {
    width:50px;

    img {
        max-width: 100%;
    }
}</style>
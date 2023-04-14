<script>
export default {
    name: 'SiteFooter',
    data() {
        return {
            listIcons: [
                '/img/footer-facebook.png',
                '/img/footer-twitter.png',
                '/img/footer-youtube.png',
                '/img/footer-pinterest.png',
                '/img/footer-periscope.png'
            ]
        }
    }
}
</script>

<template>
    <!-- Footer -->
    <footer class="py-4">
        <div class="container">
            <div class="row">
                <div class="col d-flex justify-content-between">
                    <a class="sign_up  px-2 py-1">SIGN-UP NOW!</a>
                    <div class="icon">
                        <span class="fw-bold me-3">FOLLOW US</span>
                        <img :src="icon" alt="" v-for="icon in listIcons" class="px-1">
                    </div>       
                </div>
            </div>
        </div>
    </footer>
</template>


<style lang="scss" scoped>
footer {
    background-color: #303030;

    .sign_up {
        text-decoration: none;
        border: 2px solid #0282f9;
        cursor: pointer;
        color: white;
    }

    .sign_up:hover {
        color: #02f933;
        border: 2px solid white;
    }

    .icon span {
        color:#0282f9;
    }
}
</style>
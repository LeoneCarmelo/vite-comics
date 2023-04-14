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
@use '../assets/scss/partials/variables' as *;
footer {
    background-color: $dark;

    .sign_up {
        text-decoration: none;
        border: 2px solid $blue-strip;
        cursor: pointer;
        color: $light;
    }

    .sign_up:hover {
        color: $sign-up;
        border: 2px solid $light;
    }

    .icon span {
        color:$blue-strip;
    }
}
</style>
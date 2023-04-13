<script>
export default {
    name: 'SiteFooter'
}
</script>
<template>
    <footer class="py-4">
        <div class="container">
            <div class="row">
                <div class="col d-flex justify-content-between">
                    <a class="sign_up  px-2 py-1">SIGN-UP NOW!</a>
                    <div class="icon">
                        <span class="fw-bold">FOLLOW US</span>
                        <font-awesome-icon icon="fa-brands fa-facebook" />
                        <font-awesome-icon icon="fa-brands fa-twitter" />
                        <font-awesome-icon icon="fa-brands fa-youtube" />
                        <font-awesome-icon icon="fa-brands fa-pinterest" />
                        <font-awesome-icon icon="fa-solid fa-location-dot" />
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
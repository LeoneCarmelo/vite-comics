<script>
import SiteHeader from './components/SiteHeader.vue'
import SiteMain from './components/SiteMain.vue'
import SectionStrip from './components/SectionStrip.vue'
import SectionInfo from './components/SectionInfo.vue'
import SiteFooter from './components/SiteFooter.vue'
    export default {
        components: {
            SiteHeader,
            SiteMain,
            SectionStrip,
            SectionInfo,
            SiteFooter
        }
    }
</script>

<template>

    <SiteHeader></SiteHeader>

    <SiteMain></SiteMain>

    <SectionStrip></SectionStrip>

    <SectionInfo></SectionInfo>

    <SiteFooter></SiteFooter>
    
</template>

<style lang="scss">
</style>

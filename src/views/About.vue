<template>
    <div>
        <div class="w-12/12">
            <banner :imgSrc="imgSrc"></banner>
            <h1 class="text-lg">About area</h1>
        </div>
    </div>
</template>
<script>
import Banner from '../components/layout/Banner.vue'
export default {
    components: {
        Banner
    },
    data () {
        return {
            imgSrc: require('../assets/img/banner/about.jpg')
        }
    },
}
</script>
<template>
    <div>
        <div class="w-12/12 bg-gray-900">
            <banner :imgSrc="imgSrc"></banner>
            <h1 class="text-lg">Home area</h1>
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
            imgSrc: require('../assets/img/banner/home.jpg')
        }
    },
    beforeMount() {
        // console.log(window.screen.width)
        // console.log(window.screen.height)
    },
}
</script>
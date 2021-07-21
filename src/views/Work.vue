<template>
    <div class="w-12/12">
        <banner :imgSrc="imgSrc"></banner>
        <h1 class="text-lg">Work area</h1>
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
            imgSrc: require('../assets/img/banner/work.jpg')
        }
    },
}
</script>
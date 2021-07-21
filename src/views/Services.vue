<template>
    <div>
        <div class=" w-12/12">
            <banner :imgSrc="imgSrc"></banner>
            <h1 class="text-lg bg-gray-900">Services area</h1>
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
            imgSrc: require('../assets/img/banner/services.jpg')
        }
    },
}
</script>
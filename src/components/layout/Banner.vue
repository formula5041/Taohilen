<template>
    <div class="flex justify-around items-center w-full">
        <img :src="imgSrc" class="w-full">
    </div>
</template>

<script>
    export default {
        data () {
            return {
                
            }
        },
        props: {
            imgSrc: {
                type: String,
                required: false,
                default: ''
            }
        }
    }
</script>
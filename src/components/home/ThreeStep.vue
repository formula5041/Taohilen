<template>
    <div class="flex flex-col justify-center items-center transform transition-all duration-500 hover:-translate-y-4">
        <img :src="img" :class="width">
        <span>STEP {{index}}</span>
        <div class="flex flex-col">
            <p>{{title}}</p>
            <span>{{info}}</span>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            img: {
                type: String,
                required: false,
                default: ''
            },
            index: {
                type: String,
                required: false,
                default: ''
            },
            title: {
                type: String,
                required: false,
                default: ''
            },
            info: {
                type: String,
                required: false,
                default: ''
            },
            width: {
                type: String,
                required: false,
                default: ''
            }
        }
    }
</script>
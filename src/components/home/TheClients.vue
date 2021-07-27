<template>
    <div>
        <base-title :title="'CLIENTS'"></base-title>
        <div class="border-2 flex flex-wrap justify-center mx-20">
            <a v-for="item in brand" :key="item" :href="item.link" target="_blank" class=" my-16 mx-8 transform transition-all duration-500 hover:scale-125">
                <img :src="item.img" class="w-32 h-32">
            </a>
        </div>
    </div>
</template>

<script>
    import BaseTitle from '../base/BaseTitle.vue'
    export default {
        components: {
            BaseTitle
        },
        data () {
            return {
                brand: [
                    {
                        img : require('../../assets/img/brand/brand (1).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (2).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (3).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (4).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (5).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (6).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (7).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (8).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (9).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (10).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (1).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                    {
                        img : require('../../assets/img/brand/brand (2).svg') ,
                        link: 'https://www.shazam.com/zh'
                    },
                ]
            }
        }
    }
</script>
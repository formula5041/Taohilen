<template>
    <footer class="flex w-full py-5 border-t-2 border-green-300">
        <div class="flex flex-col items-start w-3/6">
            <ul class="flex mb-2">
                <li v-for="itme in ports" :key="itme" class="mr-3">{{itme}}</li>
            </ul>
            <p class="mb-2">{{email}}</p>
            <div class="flex flex-col items-start">
                <span class="mb-2">{{companyName}}</span>
                <span>{{companyNameEn}}</span>
            </div>
        </div>
        <div class="flex flex-col items-start w-3/6">
            <h1 class="mb-2">WORK WITH US!</h1>
            <p class="text-left mb-2">
                專業，指終如一。相信，獨一無二。
            </p>
            <p class="text-left mb-2">
                認真的態度，面對每一個細節，真多元的角度，處理每一個不可能。
            </p>
            <router-arrow></router-arrow>
        </div>
    </footer>
</template>

<script>
    import RouterArrow from '../base/RouterArrow.vue'
    export default {
        components: {
            RouterArrow
        },
        data () {
            return {
                navItem: [ 
                    { name: 'About', link:'/about' },
                    { name: 'Services', link:'/services' },
                    { name: 'Work', link:'/work' },
                    { name: 'Contact', link:'/contact' },
                ],
                ports: ['龜吼漁港', '野柳漁港', '翡翠漁港'],
                email: 'formula5041@gmail.com',
                companyName: '討海人集團版權所有',
                companyNameEn: 'Copyright © TAOHILEN All Rights Reserved.'
            }
        }
    }
</script>
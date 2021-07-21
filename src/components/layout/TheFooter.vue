<template>
    <footer class="flex w-full pt-1 border-t-2 border-green-300">
        <div class="flex flex-col items-center justify-center w-3/6">
            <ul class="flex">
                <li v-for="itme in ports" :key="itme" class="ml-3">{{itme}}</li>
            </ul>
            <p>{{email}}</p>
            <div class="flex flex-col">
                <span>{{companyName}}</span>
                <span>{{companyNameEn}}</span>
            </div>
        </div>
        <div class="flex flex-col w-3/6">
            <h1>WORK WITH US!</h1>
            <p class="text-left">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nihil reiciendis eveniet illo ea vitae qui earum itaque molestiae dolor neque perspiciatis tenetur expedita culpa in, natus delectus dignissimos assumenda accusantium!
            </p>
            <div class="flex justify-center">
                <img :src="arrowImg" class="w-4 mr-2">
                <router-link to='/work' class="hover:bg-green-500">See jobs</router-link>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        data () {
            return {
                navItem: [ 
                    { name: 'About', link:'/about' },
                    { name: 'Services', link:'/services' },
                    { name: 'Work', link:'/work' },
                    { name: 'Contact', link:'/contact' },
                ],
                ports: ['龜吼漁港', '野柳漁港', '翡翠漁港'],
                arrowImg: require('../../assets/img/icon/arrow_right.svg'),
                email: 'formula5041@gmail.com',
                companyName: '討海人集團版權所有',
                companyNameEn: 'Copyright © TAOHILEN All Rights Reserved.'
            }
        }
    }
</script>
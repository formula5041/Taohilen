<template>
    <div class=" w-12/12">
        <banner :imgSrc="imgSrc"></banner>
        <div class="mx-20">
            <!-- <the-slogan></the-slogan> -->
            <div class="flex justify-around mt-12">
                <three-step
                    v-for="(item, index) in stepItems"
                    :key="index"
                    :img="item.img"
                    :index="index+1"
                    :width="'w-24'"
                    :title="item.title"
                    :info="item.info"
                >
                </three-step>
            </div>
            <the-clients class="mt-16"></the-clients>
        </div>
    </div>
</template>
<script>
import Banner from '../components/layout/Banner.vue'
import ThreeStep from '../components/home/ThreeStep.vue'
import TheClients from '../components/home/TheClients.vue'
// import TheSlogan from '../components/home/TheSlogan.vue'
export default {
    components: {
        Banner,
        TheClients,
        ThreeStep
        
    },
    data () {
        return {
            imgSrc: require('../assets/img/banner/home.jpg'),
            stepItems: [
                {
                    img : require('../assets/img/icon/home/threestep/fishing.svg') ,
                    title:'現撈魚貨',
                    info: '每日回港卸下新鮮魚貨'
                },
                {
                    img : require('../assets/img/icon/home/threestep/delivery.svg') ,
                    title:'低溫急送',
                    info: '特殊冷藏技術快速配送'
                },
                {
                    img : require('../assets/img/icon/home/threestep/package.svg') ,
                    title:'專業服務',
                    info: '優質服務品質安心交貨'
                }
            ]
        }
    },
    beforeMount() {
        // console.log(window.screen.width)
        // console.log(window.screen.height)
    },
}
</script>

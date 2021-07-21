<template>
    <nav class="flex justify-between items-center w-full pt-1">
        <router-link to="/"><img class="w-16 ml-4" src="../../assets/img/icon/fish.svg"></router-link>
        <ul class="flex mr-8">
            <li v-for="item in navItem" :key="item" class="m-4 text-gray-50 transition duration-500" :id="item.name">
                <router-link :to="item.link" >{{item.name}}</router-link>
            </li>
        </ul>
    </nav>
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
                ]
            }
        },
        beforeMount() {
            // console.log(document.querySelector('#About'))
        },
        watch : {
            $route () {
                document.querySelectorAll('li').forEach( item => {
                    item.style.backgroundColor = 'transparent'
                })
               
                const about = document.querySelector('#About')
                const services = document.querySelector('#Services')
                const work = document.querySelector('#Work')
                const contact = document.querySelector('#Contact')
                // this.$route.path === '/about' ? `${about.setAttribute("style", "background-color: #10B981;")}` : `${about.setAttribute("style", "background-color: transparent;")}`
                // this.$route.path === '/services' ? `${services.setAttribute("style", "background-color: #10B981;")}` : `${services.setAttribute("style", "background-color: transparent;")}`
                // this.$route.path === '/work' ? `${work.setAttribute("style", "background-color: #10B981;")}` : `${work.setAttribute("style", "background-color: transparent;")}`
                // this.$route.path === '/contact' ? `${contact.setAttribute("style", "background-color: #10B981;")}` : `${contact.setAttribute("style", "background-color: transparent;")}`
                switch (this.$route.path){
                    case '/about' :
                        about.setAttribute("style", "background-color: #10B981;")
                        break
                    case '/services' :
                        services.setAttribute("style", "background-color: #10B981;")
                        break
                    case '/work' :
                        work.setAttribute("style", "background-color: #10B981;")
                        break
                    case '/contact' :
                        contact.setAttribute("style", "background-color: #10B981;")
                        break                        
                }
            }
        }
    }
</script>
<template>
    <div>
        <div class="flex justify-center">
            <h1 class="text-green-500 border-b-2 border-transparent w-64 my-10 text-5xl transform transition-all duration-500 hover:border-green-200">{{title}}</h1>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['title']
    }
</script>
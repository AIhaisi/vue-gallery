<template>

    <head>
        <title>Picture</title>
    </head>
      
    <body>
        <ShowGallery :imgsPath="img"/>
    </body>
</template>
<script lang='ts' setup>
import ShowGallery from '@/components/ShowGallery.vue'
//const images = import.meta.glob('@/pages/img/*.{png,jpg,svg,gif}'); //, { eager: true }

const images = import.meta.glob('@/store/img/*.{png,jpg,svg,gif,webp}')
const img: string[] = Object.keys(images)

</script>

<style scoped>
</style>
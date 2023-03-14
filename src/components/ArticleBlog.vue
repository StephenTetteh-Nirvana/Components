<template>
  <h2>{{ title }}</h2>
  <h2>Likes-{{ likes }}</h2>
  <h2>Published-{{ isPublished ? 'Yes' : 'No' }}</h2>
 
  
</template>

<script>
    export default {
        props:{
            title:String,
            likes:Number,
            isPublished:Boolean,
        },
        
    }
</script>

<style scoped>

</style>
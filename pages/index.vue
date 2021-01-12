<template>
  <h1>Welcome to my first nuxt app</h1>
</template>



<script>
export default {
    head(){
        return{
            title: 'Home | Nuxt App',
            meta:[
                {
                    hid: 'description',
                    name: 'description',
                    content: 'Website Home'
                }
            ],
            htmlAttrs:{
                lang:'en'
            }
        }
    }
}
</script>
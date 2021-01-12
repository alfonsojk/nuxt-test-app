<template>
    <h1>Editing</h1>
</template>

<script>
import axios from 'axios'
export default {
    data (){
        return {
            post:{}
        }
    },
    async created() {
       const res = await axios.get('https://jsonplaceholder.typicode.com/posts/' + this.$route.params.id)
       console.log(res)
    }
}
</script>
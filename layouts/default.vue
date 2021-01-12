<template>
<div>
  <Navigation />
  <div class="content">
    <nuxt/>
  </div>
</div>
</template>

<script>
import Navigation from '../components/Navigation'
export default {
  components:{
    Navigation
  }
}
</script>

<style>
*{
  box-sizing:border-box;
  color:whitesmoke;
}
body{
  background:rgb(68, 68, 75);
  color:whitesmoke;
  font-family: Arial, Helvetica, sans-serif;
  padding-top:0;

}

.content{
  padding:2rem; 
}

</style>

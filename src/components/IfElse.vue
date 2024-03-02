<template>
   <h1 v-if="show">I am yeasin arafat</h1>
   <h1 v-else>I am else</h1>
</template>

<script>
    export default{
        name:"Home",
        data(){
            return{
                show:false
                
            }
        },
        methods:{
          
        }
    }
</script>


<style scoped>
h1{
    color:orange;
}
</style>
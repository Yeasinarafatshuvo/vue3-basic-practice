<template>
   <div v-html="tag1">

   </div>
</template>

<script>

export default{
    name:"Home",
    components:{
        
    },
    data(){
        return{
           tag1:"<h1>I am from html tag</h1>"
        }
    },
    methods:{
        
    }
}
</script>


<style scoped>

</style>
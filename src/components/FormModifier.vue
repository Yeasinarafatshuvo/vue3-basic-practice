<template>
<input type="text" v-model.trim="name">
<p>{{ name }}</p>
</template>

<script>
export default{
    name:"Home",
    components:{
        
    },
    data(){
        return{
            name:""
        }
    },
    methods:{
      
    }
}
</script>


<style scoped>
.green{
    color:green
}
</style>
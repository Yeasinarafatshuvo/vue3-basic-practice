<template>
   <button @click="tag = 'Java'">Java</button>
   <button @click="tag = 'Php'">Php</button>

    <component :is="tag"></component>
</template>

<script>
import Php from "./Php.vue";
import Java from "./Java.vue"
export default{
    name:"Home",
    components:{
        Php,
        Java
    },
    data(){
        return{
            tag:'Java'
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
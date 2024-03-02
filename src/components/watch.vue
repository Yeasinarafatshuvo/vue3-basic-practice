<template>
    <h1>{{count}}</h1>
    <button @click="count = count + 1">+</button>
    <button @click="count = count - 1">-</button>
</template>

<script>
export default{
    name:"Home",
    components:{
        
    },
    data(){
        return{
           count:0
        }
    },
    watch:{
        count(val, prev){
            if(val > 5 && val > prev){
                this.count = 0;
            }
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
<template>
   <Child name="I am from child" :user="user"  :getdata="getdata"/>
</template>

<script>
import Child from "./Child.vue"
export default{
    name:"Home",
    components:{
        Child
    },
    data(){
        return{
         user:{name:"Yeasin", email:"yeasin@gmail.com"}   
        }
    },
    methods:{
        getdata(){
            alert("I am from parents");
        }
    }
}
</script>


<style scoped>

</style>
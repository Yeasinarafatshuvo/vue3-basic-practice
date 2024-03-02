<template>
    <input type="text" placeholder="Enter Email" v-model="email">
    <br>
    <input type="text" placeholder="Enter Password" v-model="password">
    <br>
    <button @click="getData()">save</button>
</template>

<script>
    export default{
        name:"Home",
        data(){
            return{
                email:null,
                password:null
                
            }
        },
        methods:{
           getData(){
            alert(`Email: ${this.email} Password: ${this.password}`);
           }
        }
    }
</script>


<style scoped>
h1{
    color:orange;
}
</style>
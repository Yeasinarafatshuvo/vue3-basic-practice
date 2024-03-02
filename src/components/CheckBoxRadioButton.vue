<template>
    <label for="php">php</label>
    <input type="checkbox" value="php" v-model="technology" id="php">

    <label for="node">node</label>
    <input type="checkbox" value="node" v-model="technology" id="node">

    <label for="java">java</label>
    <input type="checkbox" value="java" v-model="technology" id="java">
    <p>{{ technology }}</p>

    <label for="student">student</label>
    <input type="radio" value="student" v-model="who" id="student">

    <label for="node">developer</label>
    <input type="radio" value="developer" v-model="who" id="developer">
    <p>{{ who }}</p>
</template>

<script>
    export default{
        name:"Home",
        data(){
            return{
                technology:[],
                who:null
                
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
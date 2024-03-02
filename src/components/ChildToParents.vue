<template>
    <div>
        <h1>User Component</h1>
        <button @click="getUserName(userName)">Send User Name</button>
    </div>
</template>

<script>
export default{
    name:"ChildToParents",
    props:{
        getUserName:Function
    },
    data(){
        return{
            userName:"Yeasin Arafat"
        }
    }
}
</script>

<style>

</style>
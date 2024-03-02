<template>
    <h1>{{ name }}</h1>
    <p>{{ user.name }}</p>
    <p>{{ user.email }}</p>
    <button @click="getdata()">Get Data</button>
</template>

<script>
export default{
    name:"Child",
    props:{
        name:String,
        user:Object,
        getdata:Function
    }
}
</script>

<style scoped>

</style>
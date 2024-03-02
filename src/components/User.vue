<template>
    <h1>Reuse Component</h1>
    <div class="user">
        <p>{{ data.name }}</p>
        <p>{{ data.email }}</p>
        <button @click="getdata()">alert</button>
    </div>
</template>

<script>
export default{
    name:"User",
    props:{
        data:Object,
        getdata:Function
    }
}
</script>

<style scoped>
.user{
    background-color: aqua;
}
</style>
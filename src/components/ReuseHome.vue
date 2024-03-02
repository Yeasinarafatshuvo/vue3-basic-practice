<template>
    <ul>
        <li v-for="item in users" :key="item.name">
            <User :data="item" :getdata="getdata"/>
        </li>
    </ul>
</template>

<script>
import User from "./User.vue"

export default{
    name:"Home",
    components:{
        User
    },
    data(){
        return{
            users: [
                {
                    name:"yeasin",
                    email:"yeasin@gmail.com"
                },
                {
                    name:"arafat",
                    email:"arafat@gmail.com"
                },
                {
                    name:"shuvo",
                    email:"shuvo@gmail.com"
                }
            ]
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
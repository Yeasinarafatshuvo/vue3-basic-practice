<template>
    <h1>Home Component {{10 + 10}}</h1>
    <p>{{ email }}</p>
    <p>{{ getname("yeasin") }}</p>
    <p>{{ getdata().name  }} and {{ getdata().email }}</p>
    <button @click="getCount()">click</button>
    <button>{{ count }}</button>
</template>

<script>
    export default{
        name:"Home",
        data(){
            return{
                email: "yeasin@gmail.com",
                count:0,
                
            }
        },
        methods:{
            getname(a){
                return a;
            },
            getdata(){
                return {
                    name:"yeasin",
                    email:this.email
                }
            },
            getCount(){
                this.count += 1;
            }
        }
    }
</script>


<style scoped>
h1{
    color:orange;
}
</style>
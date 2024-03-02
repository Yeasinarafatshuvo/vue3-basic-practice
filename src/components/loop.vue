<template>
   <li v-for="item in technology" :key="item">
    {{ item }}
   </li>
   <br>
   <br>
   <br>
   <ul>
    <li v-for="item in users" :key="item.email">
        {{ item.name }} {{ item.email }}
    </li>
   </ul>
</template>

<script>
    export default{
        name:"Home",
        data(){
            return{
                technology:['php', 'javascript', 'laravel', 'java'],
                users:[
                    {
                        name:'yeasin',
                        email:'yeasin@gmail.com'
                    },
                    {
                        name:'arafat',
                        email:'arafat@gmail.com'
                    }
                ]
                
            }
        },
        methods:{
          
        }
    }
</script>


<style scoped>
h1{
    color:orange;
}
</style>
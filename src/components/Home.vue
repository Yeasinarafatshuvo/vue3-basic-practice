<template>
    <button @click="show = !show">Toggle</button>
    <BeforeUnmountMount v-if="show" />
 </template>
 
 <script>
 import BeforeUnmountMount from './BeforeUnmountMount.vue';
 export default{
     name:"Home",
     components:{
        BeforeUnmountMount
     },
     data(){
         return{
            show:true
         }
     },
 
   
     methods:{
         
     }
 }
 </script>
 
 
 <style scoped>
 </style>
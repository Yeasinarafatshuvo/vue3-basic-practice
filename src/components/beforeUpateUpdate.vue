<template>
    <h1 ref="count">{{ counter }}</h1>
    <button @click="counter = counter + 1">Update Count</button>
 </template>
 
 <script>
 export default{
     name:"Home",
     components:{
        
     },
     data(){
         return{
             counter:0
         }
     },
 
     beforeUpdate(){
        console.warn("beforeUpdated", this.$refs['count'].textContent);
     },
     updated(){
         console.warn("Mounted", this.counter);
     },
     methods:{
         
     }
 }
 </script>
 
 
 <style scoped>
 </style>
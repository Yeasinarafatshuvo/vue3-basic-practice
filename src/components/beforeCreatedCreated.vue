<template>
   <h1>beforeCreated and Created {{ name }}</h1>
</template>

<script>
export default{
    name:"Home",
    components:{
       
    },
    data(){
        console.warn("created");
        return{
            name:"Anil"
        }
    },

    beforeCreate(){
        this.name = "arafat";
        alert("Before Create");
    },
    created(){
        this.name = "yeasin";
        alert("Created");
    },
    methods:{
        
    }
}
</script>


<style scoped>
.green{
    color:green
}
</style>
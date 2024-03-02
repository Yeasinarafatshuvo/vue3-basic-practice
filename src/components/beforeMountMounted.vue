<template>
   <h1>BeforeMount and Mounted {{ name }}</h1>
   <h1>Code step by step</h1>
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

    beforeMount(){
       console.warn("beforeMount", this.$el);
    },
    mounted(){
        console.warn("Mounted", this.$el);
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
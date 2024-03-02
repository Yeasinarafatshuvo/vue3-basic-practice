<template>
    <h1>Computed Property</h1>
    <p>{{ getResult }}</p>
</template>

<script>
export default{
    name:"Home",
    components:{
        
    },
    data(){
        return{
           dollar:100,
           rupesval: 70,
           discount:10
        }
    },
    methods:{
        
    },
    computed:{
        getResult()
        {
            return (this.dollar * this.rupesval) - this.discount;
        }
    }
}
</script>


<style scoped>
.green{
    color:green
}
</style>
<template>
<input type="text" ref="input">
<button @click="getData()">click</button>
</template>

<script>
export default{
    name:"Home",
    components:{
        
    },
    data(){
        return{

        }
    },
    methods:{
      getData(){
        this.$refs.input.focus();
        let value = this.$refs.input.value;
        this.$refs.input.color="red";
        alert(value);
      }
    }
}
</script>


<style scoped>
.green{
    color:green
}
</style>
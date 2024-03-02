<template>
  <p :class="{green:colorful}">My name is yeasin arafat shuvo</p>
</template>

<script>

export default{
    name:"Home",
    components:{
        
    },
    data(){
        return{
            colorful:true
        }
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
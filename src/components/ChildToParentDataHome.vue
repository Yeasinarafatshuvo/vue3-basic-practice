<template>
<h1>Send data Child to parents</h1>
<ChildToParents :getUserName="getUserName" />
<h1>{{ childUser }}</h1>
</template>

<script>
import ChildToParents from './ChildToParents.vue';
export default{
    name:"Home",
    components:{
        ChildToParents
    },
    data(){
        return{
            childUser:""
        }
    },
    methods:{
      getUserName(name){
        this.childUser = name;
        alert(name);
      }  
    }
}
</script>


<style scoped>
.green{
    color:green
}
</style>
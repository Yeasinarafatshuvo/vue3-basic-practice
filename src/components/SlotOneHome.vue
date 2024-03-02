<template>
    <SlotOne>
        <h1>This is slot one</h1>
        <img src="https://images.assetsdelivery.com/compings_v2/maaravic/maaravic2210/maaravic221000257.jpg" alt="">
    </SlotOne>
</template>

<script>
import SlotOne from './SlotOne.vue';
export default{
    name:"Home",
    components:{
        SlotOne
    },
    data(){
        return{
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
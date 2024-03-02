<template>
    <SlotTwo>
        <template v-slot:header>
            <h1>Yeasin Arafat</h1>
        </template>
        <template v-slot:content>
            <button>Buy Now</button>
        </template>
        <template v-slot:footer>
            <p>A vue js products</p>
        </template>
    </SlotTwo>
</template>

<script>
import SlotTwo from './SlotTwo.vue';

export default{
    name:"Home",
    components:{
        SlotTwo
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
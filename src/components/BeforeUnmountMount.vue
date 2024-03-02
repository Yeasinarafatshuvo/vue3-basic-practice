<template>
    <div>
        <h1 ref="user">Before Unmount And Mount</h1>
    </div>
</template>

<script>
export default{
    name:"BeforeUnmountMount",
    beforeUnmount(){
        console.log("BeforeUnmount", this.$refs['user']);
    },
    unmounted(){
        console.log("unmounted", this.$refs['user']);
    }
}
</script>
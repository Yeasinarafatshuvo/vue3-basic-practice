<template>
    <div class="cart">
        <header>
            <slot name="header"></slot>
        </header>
        <content>
            <slot name="content"></slot>
        </content>
        <footer>
            <slot name="footer"></slot>
        </footer>
    </div>
</template>

<script>
export default{
    name:"SlotTwo"
}
</script>

<style scoped>
.cart{
    border: 1px solid black;
    text-align: center;
}
</style>
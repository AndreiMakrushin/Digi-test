<script setup>
import CardProduct from './productContainerComponents/CardProduct.vue';
</script>

<template>
    <div class="Products-container">
        <CardProduct />
        <CardProduct />
        <CardProduct />
        <CardProduct />
        <CardProduct />
        <CardProduct />
        <CardProduct />
        
    </div>
</template>



<style  scoped>
.Products-container {
    width: 100%;
    display: grid;
    gap: 24px;
    grid-template-columns: repeat(4, 1fr);
}


</style>
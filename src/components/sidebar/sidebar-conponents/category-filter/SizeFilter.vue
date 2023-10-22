<script setup>
    import CheckboxConteiner from '../../../ui/sidebar/CheckboxConteiner.vue';
</script>
<template>
    <div class="size-container">
        <div class="header">
            <h1>Размер</h1>
        </div>
        <CheckboxConteiner /> 
        </div>    
</template>
<style scoped>
    .size-container{
        margin-top: 16px;
        width: 100%;
        display: flex;
        flex-direction: column;
    }
    .header{
        text-align: center;
    }
    .header h1{
        font-weight: 700;
        font-size: 16px;
        line-height: 20px;
    }
</style>
    

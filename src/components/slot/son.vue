<template>
    <div>
        <h1>今天的天气是：</h1>
        <slot name="temp"></slot>
        <h1>心情：</h1>
        <slot name="mind"></slot>
    </div>
</template>

<script>
    export default {
        name: "son"
    }
</script>

<style scoped>

</style>
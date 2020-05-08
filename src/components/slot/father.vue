<template>
    <div>
        <son>
            <p slot="temp">38C°</p>
            <p slot="mind">心情不错</p>
        </son>
    </div>
</template>

<script>
    import son from "@/components/slot/son";

    export default {
        name: "father",
        components: {
            "son": son
        }
    }
</script>

<style scoped>

</style>
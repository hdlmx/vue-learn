<template>
    <div>{{msg}}
        <h1>当前数字</h1>
        {{published}}
    </div>

</template>

<script>
    export default {
        name: "son",
        props: {
            msg: {
                type: String
            },
            published: {
                type: String
            }

        }
    }
</script>

<style scoped>

</style>
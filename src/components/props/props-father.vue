<!--在vue中，如果父组件向子组件传递数据时通过props实现
1、在子组件中申明props属性，指明接受父组件的变量：
            props: {
                 msg: String
              }
 2、父组件在调用的时候，在子组件标签上声明子组件props中生命的变量：
             <son msg="hello world"></son>

-->
<template>
    <div>
        <son msg="hello world" :published="num"></son>
        <button @click="change">点击</button>
    </div>
</template>

<script>
    import son from "@/components/props/props-son";

    export default {
        name: "father",
        data() {
            return {
                num: 1
            }
        },
        components: {
            "son": son
        },
        methods: {
            change() {
                this.num++;
            }
        }
    }
</script>

<style scoped>

</style>
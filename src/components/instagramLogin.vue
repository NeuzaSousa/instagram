<template>
    <div>
        <h1>Hello from login</h1>
        <h2>The count is: {{ count }}</h2>
        <button @click="count++">+1</button>
    </div>
</template>

<script>
export default{
    data(){
        return{
            count: 0
        };
    }
};
</script>

<style scoped>

</style>

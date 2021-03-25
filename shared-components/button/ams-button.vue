<template>
    <button @click="$emit('dostuff')" v-text="label"></button>
</template>

<style scoped>
button {
    display: inline-block;
    background: #37e031;
    color: #fff;
    border: 1px solid #bbb;
    border-radius: 4px;
    padding: 10px 20px;
    margin: 4px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
</style>

<script>
export default {
    name: "AmsButton",
    props: {
        label: String
    },
    emits: ["dostuff"]
}
</script>

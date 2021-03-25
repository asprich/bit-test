<template>
    <button @click="$emit('dostuff')" v-text="label"></button>
</template>

<script>
export default {
    name: "AmsButton",
    props: {
        label: String
    },
    emits: ["dostuff"]
}
</script>

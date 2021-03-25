<template>
    <div v-text="text"></div>
</template>

<script>
export default {
    name: "AmsMessageDisplay",
    props: {
        text: String
    }
}
</script>
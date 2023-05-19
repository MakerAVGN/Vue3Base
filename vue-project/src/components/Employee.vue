<script>
export default {
    props: {
        name: String,
        surn: String,
        age: Number
    },
    data() {
        return {

        }
    }
}
</script>
<template>
    {{ name }}
    {{ surn }}
    {{ age }}
</template>
<script>

export default {
props: {
    buttonText: String
}
}
</script>
<template>
<button>{{ buttonText }}</button>

</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
button {
    background-color: $green-color;
    border: none;
    border-radius: 1rem;
    padding: 5px;
    width: 100px;
    color: white;
    font-size: .8rem;
}
</style>
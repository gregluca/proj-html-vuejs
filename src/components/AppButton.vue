<script>

export default {
props: {
    buttonText: String
}
}
</script>
<template>
<button><a href="">{{ buttonText }}</a></button>

</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
button {
    background-color: $green-color;
    border: none;
    padding: 10px;
    border-radius: 1rem;
    letter-spacing: 1px;
    width: 50%;

    a {
        text-decoration: none;
        color: white;
    }
}
</style>
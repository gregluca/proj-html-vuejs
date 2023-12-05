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
    width: 70%;
    background-color: $green-color;
    border: none;
    padding: 10px;
    border-radius: 1rem;
    letter-spacing: 1px;
    font-size: .6rem;

    a {
        text-decoration: none;
        color: white;
    }
}
button:hover {
    opacity: .8;
    background-color: black;
    color: $green-color;
}
</style>
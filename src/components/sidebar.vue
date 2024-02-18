<script setup>
const sbcontent = [["APP", "/app"], ["GO", "/go"], ["item", "/item"]]

</script>
<template>
    <div>
        <ul id="sidebar">
            <li v-for="items in sbcontent"><a :href=items[1] >{{ items[0] }}</a></li>
        </ul>
    </div>
</template>
<style scoped>
#sidebar {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1rem;
    padding-left: 0;
}

#sidebar li {
    list-style-type: none;
    background-color: brown;
    width: 80%;
    padding: 1rem;
    text-align: center;
    border-radius: 1rem;
}

#sidebar a {
    text-decoration: none;
    color: black;
}

</style>
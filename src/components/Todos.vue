<template>
    <div>
        <li>{{ todos.text }}</li>
    </div>
</template>


<script>
    export default {
        name: "Todos",
        props: ['todos'],
    }
</script>

<style scoped>

</style>
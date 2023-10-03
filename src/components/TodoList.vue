<script>
export default {
    props: {
        todos: {
            type: Array
        }
    }
}
</script>

<template>

    <div>
        <ol>
            <li v-for="todo in todos">{{ todo }}</li>
        </ol>
    </div>

</template>
<script>

    export default {
        data() {
            return {
                count: 0
            }
        },
        methods: {
            increase() {
                this.count++
            },
            decrease() {
                this.count--
            }
        }
    }
</script>

<template>
    <div>
        <p>{{ count }}</p>
        <button v-on:click="increase">+</button>
        <button v-on:click="decrease">-</button>
    </div>
</template>
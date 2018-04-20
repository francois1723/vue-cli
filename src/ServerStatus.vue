<template>
    <div class="wrapper">
        <h3>ServerStatus.vue</h3>
        <p>Server status: {{ status }}</p>
        <hr>
        <button @click="changeStatus">Change status</button>
    </div>
</template>

<script>
    export default {
        data: function() {
            return {
                status: 'Critical'
            }
        },
        methods: {
            changeStatus() {
                this.status = 'Normal';
            }
        }
    }

</script>

<style>
    .wrapper {
        border: 1px solid black;
        padding: 0 1em 1em 1em;
        max-width: 20%;
    }

</style>

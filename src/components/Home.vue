<template>
    <div>
        <h1>Trade or View your Porfolio</h1>
        <h6>You may Save and Load your Data</h6>
        <h6>Click to end your day</h6>
        <p>Your funds: {{funds | currency}}</p>
    </div>
</template>

<script>
    export default {
        computed: {
            funds() {
                return this.$store.getters.funds;
            }
        }
    }
</script>
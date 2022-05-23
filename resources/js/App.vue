<template>
    <br>
    <hr>
    Hello VueJS!
    <hr>
    <CounterButton :startv="12" :min="1" :max="13"></CounterButton>
    <br>
    <counter-button :startv="2"></counter-button>
</template>

<script>
import CounterButton from "./components/CounterButton";

export default {
    name: "App.vue",
    components: {
        CounterButton
    }
}
</script>

<style scoped>

</style>

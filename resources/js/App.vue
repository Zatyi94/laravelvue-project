<template>
    <br>
    <hr>
    Hello VueJS!
    <hr>
    <CounterButton :startv="12" :min="1" :max="13"></CounterButton>
    <br>
    <counter-button :startv="2"></counter-button>
    <hr>
    <hr>
    <TemplateBox></TemplateBox>
</template>

<script>
import CounterButton from "./components/CounterButton";
import TemplateBox from "./components/TemplateBox";

export default {
    name: "App.vue",
    components: {
        CounterButton,
        TemplateBox
    }
}
</script>

<style scoped>

</style>

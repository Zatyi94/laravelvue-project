<template>
    <button @click="decrement"> - </button>
    {{ number }}
    <button @click="increment"> + </button>
    <button @click="number=startValue"> Clear </button>
</template>

<script>
export default {
    name: "CounterButton",
    /* props: ['startv', 'min', 'max'], // jelzem a komponensemnek, hogy számítson vmilyen paraméterre */
    props: {
        startv: Number,
        min: {
            type: Number,
            default: 0
        },
        max: {
            type: Number,
            default: 15
        }
    },
    data() {
        return {
            number: isFinite(this.startv) ? this.startv : 0
        };
    },
    computed: { // adattagok
        startValue(){
            return isFinite(this.startv) ? this.startv : 0;
        }
    },
    methods: {
      increment(){
          console.log(this.max);
          if (this.number < this.max){
              this.number++;
          }
      },
      decrement(){
          if (this.number > this.min){
              this.number--;
          }
      }
    }
}
</script>

<style scoped>

</style>

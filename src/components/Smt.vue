<template>
  <div class="smt">
    Smt: {{msg}}!
    <p>[Store] Counter: {{count}}</p>
    <p>
      <button @click="increment">+</button>
      <button @click="decrement">-</button>
    </p>
  </div>
</template>

<script>


export default {
  name: "Smt",
  props: {
    msg: String
  },
  computed: {
    count() {
      return this.$store.state.counter;
    }
  },
  methods: {
    increment() {
      this.$store.commit("increment");
    },
    decrement() {
      this.$store.commit("decrement");
    }
  }
};
</script>

<style scoped>
.smt {
  border: 1px dashed darksalmon;
}
</style>
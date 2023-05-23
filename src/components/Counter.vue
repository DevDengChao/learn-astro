<template>
  <div>
    Vue Count
    <button @click="countDown">-</button>
    {{ count }}
    <button @click="countUp">+</button>
  </div>
</template>
<script>
import {defineComponent} from "vue";

export default defineComponent({
  data() {
    return {
      count: 0
    }
  },
  methods: {
    countDown() {
      this.count--;
    },
    countUp() {
      this.count++;
    },
  }
})
</script>

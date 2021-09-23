<template>
  <div>
    {{ number }}
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const number = ref(0);

    setInterval(() => {
      number.value++;
    }, 1000);
    return { number };
  },
};
</script>

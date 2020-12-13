<template>
  <div id="Parent">
    <Child :productInCart="cart" @increment="handleIncrement" @decrement="handleDecrement" />
  </div>
</template>

<script>
import Child from "./Child.vue";

export default {
  name: "Parent",
  components: {
    Child,
  },
  data() {
    return {
      cart: 0,
    };
  },
  methods: {
    handleIncrement() {
      this.cart += 1;
    },
    handleDecrement() {
      this.cart -= 1;
    },
  },
};
</script>

<style>
</style>

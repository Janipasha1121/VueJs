<template>
  <div class="Child">
      <h1>Parent↔Child Communication</h1>
    <p class="p-3 mb-2 bg-warning text-dark">Your Value is: {{ productInCart }}</p>
    <b-button class="mr-3" variant="outline-warning"  @click="$emit('increment')">Increse</b-button>&nbsp;
    <b-button class="mr-3" variant="outline-warning" @click="$emit('decrement')">Decrease</b-button>
  </div>
</template>

<script>
export default {
  name: "Child",
  props: {
    productInCart: Number
  }
};
</script>
<style>
</style>

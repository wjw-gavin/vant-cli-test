<template>
  <button class="demo-button">
    <slot />
  </button>
</template>

<script setup lang="ts">
const props = defineProps({
  color: String,
  type: {
    type: String,
    default: 'primary',
  },
})

console.log(props);

</script>

<style lang="scss">
.demo-button {
  min-width: 120px;
  color: #fff;
  font-size: 16px;
  line-height: 36px;
  background-color: #f44;
  border: none;
  border-radius: 30px;
}
</style>

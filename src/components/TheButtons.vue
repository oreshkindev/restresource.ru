<script setup lang="ts">
import { defineProps } from "vue"

interface Button {
  title: string
  state?: boolean
}

defineProps<Button>()
</script>

<template>
  <button :class="{ state: state }">{{ title }}</button>
</template>

<style scoped lang="scss">
button {
  &.state {
    border: 1px solid #000;
    border-radius: 50px;
    padding: 5px 20px;
    transition: 0.2s ease-in-out;

    &:hover {
      background: #000;
      color: #fff;
    }
  }
}
</style>

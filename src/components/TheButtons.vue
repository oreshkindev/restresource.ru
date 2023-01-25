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
    background: #000;
    border-radius: 50px;
    color: #fff;
    padding: 5px 20px;
  }
}
</style>

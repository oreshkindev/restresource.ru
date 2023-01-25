<script setup lang="ts">
import { defineProps } from "vue"

interface News {
  date: string
  descr: string
}

defineProps<News>()
</script>

<template>
  <article>
    <span>{{ date }}</span>

    <p>
      {{ descr }}
    </p>
  </article>
</template>

<style scoped></style>

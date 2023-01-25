<script setup lang="ts">
import { defineProps } from "vue"

interface Adds {
  title: string
  descr?: string
  image: string
}

defineProps<Adds>()
</script>

<template>
  <article>
    <picture>
      <source :srcset="require('@/assets/images/' + image + '.webp')" type="image/webp" />

      <img decoding="async" :src="require('@/assets/images/' + image + '.webp')" :alt="title" />
    </picture>

    <h3>{{ title }}</h3>

    <p>
      {{ descr }}
    </p>
  </article>
</template>

<style scoped></style>

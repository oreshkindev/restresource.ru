<script lang="ts" setup>
import { defineProps } from "vue"

interface PostCard {
  title: string
  descr?: string
  image?: string
  covered?: boolean
}

defineProps<PostCard>()
</script>

<template>
  <article :class="{ covered: covered }" :style="covered ? { backgroundImage: 'url(' + require('@/assets/images/' + image + '.webp') + ')' } : ''">
    <picture v-if="!covered">
      <source :srcset="require('@/assets/images/' + image + '.webp')" type="image/webp" />

      <img decoding="async" :src="require('@/assets/images/' + image + '.webp')" :alt="title" />
    </picture>

    <h3>
      <span>Идеи</span>

      {{ title }}
    </h3>

    <p>
      {{ descr }}
    </p>
  </article>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
article {
  background-size: cover;

  &.covered {
    color: #ffffff;
    display: grid;
    padding: 40px 20px;
    min-height: 600px;
    place-content: end;
  }

  picture {
    img {
      display: block;
    }
  }

  h3 {
    font-size: 24px;
    margin: 10px 0;

    span {
      display: block;
      font-size: initial;
      margin: 10px 0;
    }
  }

  p {
    word-wrap: break-word;
  }
}
</style>

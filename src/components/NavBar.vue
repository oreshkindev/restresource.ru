<script setup lang="ts">
import { defineEmits } from "vue"

const emits = defineEmits(["close"])
</script>

<template>
  <section>
    <nav>
      <i class="icon-close" @click="$emit('close')" />

      <a href="#">О проекте</a>
      <a href="#">Информационная база</a>
      <a href="#">Статьи</a>
      <a href="#">Новости</a>
      <a href="#">Рецепты</a>
      <a href="#">Идеи</a>
    </nav>
  </section>
</template>

<style scoped lang="scss">
section {
  background: rgba(0, 0, 0, 0.674);
  position: absolute;
  inset: 0;

  i {
    font-size: 30px;
    position: absolute;
    top: 20px;
    left: 20px;
  }

  nav {
    align-items: center;
    background: rgb(112, 112, 112);
    color: #fff;
    display: flex;
    flex-direction: column;
    gap: 20px;
    justify-content: center;
    padding: 300px;
    position: fixed;
    inset: 33%;
  }
}
</style>

<script lang="ts" setup>
import NewsArticle from "@/components/NewsArticle.vue"
import PostCard from "@/components/PostCard.vue"
import TheButtons from "@/components/TheButtons.vue"

const items = [
  {
    id: 1,
    date: "22:30",
    descr:
      "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ad iste repellendus fugit. Rerum, facilis asperiores? Fugiat enim, delectus, itaque sed nostrum, cupiditate vero dolorem dolore corporis hic?",
  },
  {
    id: 2,
    date: "20:30",
    descr: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. ",
  },
  {
    id: 3,
    date: "21:00",
    descr: "Rerum, facilis asperiores? Fugiat enim, delectus, odio reiciendis quia itaque sed nostrum, cupiditate vero dolorem dolore corporis hic?",
  },
  {
    id: 4,
    date: "19:27",
    descr: "odio reiciendis quia itaque sed nostrum, cupiditate vero dolorem dolore corporis hic?",
  },
]
</script>

<template>
  <div class="container">
    <section class="container__news">
      <h3>Новости</h3>

      <NewsArticle v-for="i in items" :key="i.id" :date="i.date" :descr="i.descr" />
    </section>

    <section class="container__content">
      <PostCard
        title="Anita Austvika"
        descr="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ad iste repellendus fugit. Rerum, facilis asperiores? Fugiat enim, delectus, odio reiciendis quia itaque sed nostrum, cupiditate vero
      dolorem dolore corporis hic?"
        image="anita-austvika-mBVDi_cmkOg-unsplash"
        covered
      />

      <PostCard
        title="Anita Austvika"
        descr="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ad iste repellendus fugit. Rerum, facilis asperiores? Fugiat enim, delectus, odio reiciendis quia itaque sed nostrum, cupiditate vero
      dolorem dolore corporis hic?"
        image="anita-austvika-mBVDi_cmkOg-unsplash"
      />

      <PostCard
        title="Anita Austvika"
        descr="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ad iste repellendus fugit. Rerum, facilis asperiores? Fugiat enim, delectus, odio reiciendis quia itaque sed nostrum, cupiditate vero
      dolorem dolore corporis hic?"
        image="anita-austvika-mBVDi_cmkOg-unsplash"
      />

      <PostCard
        title="Anita Austvika"
        descr="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ad iste repellendus fugit. Rerum, facilis asperiores? Fugiat enim, delectus, odio reiciendis quia itaque sed nostrum, cupiditate vero
dolorem dolore corporis hic?"
        image="anita-austvika-mBVDi_cmkOg-unsplash"
        covered
      />

      <TheButtons title="Показать еще " state />
    </section>
  </div>
</template>

<style lang="scss">
.container {
  display: flex;
  flex-wrap: wrap;
  flex: 1;
  gap: 20px;

  &__news {
    display: flex;
    flex: 0 1 20%;
    flex-direction: column;
    gap: 20px;
    // padding: 0 40px;
  }

  &__content {
    align-content: flex-start;
    display: flex;
    flex: 1;
    flex-grow: 1;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;

    article {
      flex: 1;

      &:nth-child(3n + 1) {
        flex: 100%;
      }
    }
  }
}
</style>

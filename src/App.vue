<script lang="ts" setup>
import TheButtons from "@/components/TheButtons.vue"
import TheLogo from "@/components/TheLogo.vue"
import AdBlocks from "@/components/AdBlocks.vue"
</script>

<template>
  <header>
    <nav>
      <div></div>

      <TheLogo />

      <TheButtons title="Войти" />
      <TheButtons title="Регистрация" state />
    </nav>

    <nav>
      <button>==</button>

      <a href="#">О проекте</a>
      <a href="#">Информационная база</a>
      <a href="#">Статьи</a>
      <a href="#">Новости</a>
      <a href="#">Рецепты</a>
      <a href="#">Идеи</a>

      <form action="#">
        <input type="text" placeholder="Поиск" />
      </form>
    </nav>
  </header>

  <router-view />

  <aside>
    <AdBlocks
      image="anita-austvika-mBVDi_cmkOg-unsplash"
      title="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!"
      descr="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta eligendi
      placeat amet nulla quia et doloremque?"
    />

    <AdBlocks
      image="anita-austvika-mBVDi_cmkOg-unsplash"
      title="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!"
      descr="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta eligendi
      placeat amet nulla quia et doloremque?"
    />

    <AdBlocks
      image="anita-austvika-mBVDi_cmkOg-unsplash"
      title="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!"
      descr="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta eligendi
      placeat amet nulla quia et doloremque?"
    />
  </aside>

  <footer>
    <div>
      <TheLogo color />

      <router-link to="/" :text="'email@email.ru'" />

      <nav class="social">
        <router-link to="/" href="https://ru.wikipedia.org/wiki/HTML" target="_blank">
          <img src="@/assets/logo.png" alt="/" />
        </router-link>

        <router-link to="/" href="https://ru.wikipedia.org/wiki/HTML" target="_blank">
          <img src="@/assets/logo.png" alt="/" />
        </router-link>

        <router-link to="/" href="https://ru.wikipedia.org/wiki/HTML" target="_blank">
          <img src="@/assets/logo.png" alt="/" />
        </router-link>

        <router-link to="/" href="https://ru.wikipedia.org/wiki/HTML" target="_blank">
          <img src="@/assets/logo.png" alt="/" />
        </router-link>
      </nav>
    </div>

    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia fugiat eius perspiciatis nam neque? Natus, accusantium. Amet vel autem repellendus totam neque, asperiores iure non nostrum,
      natus vitae similique, ipsam delectus enim tenetur? Fugiat quisquam magnam, molestias consequatur autem illo dolor tenetur laborum reiciendis impedit quos consectetur inventore iusto mollitia
      delectus est harum? Placeat ducimus mollitia qui vel ipsam consectetur aut minus nemo dicta explicabo in sint quos sapiente, quisquam facilis! Consequatur facilis ullam, quidem amet distinctio
      magni nisi. Sed.
    </p>

    <nav class="info">
      <router-link to="/" :text="'lorem ipsum'" />
      <router-link to="/" :text="'lorem ipsum'" />
      <router-link to="/" :text="'lorem ipsum'" />
    </nav>
  </footer>
</template>

<style lang="scss">
/* Reset and base styles  */

* {
  border: none;
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

:focus,
:active {
  outline: none;
}

a:focus,
a:active {
  outline: none;
}

/* Links */

a,
a:link,
a:visited {
  color: inherit;
  text-decoration: none;
  /* display: inline-block; */
}

a:hover {
  /* color: inherit; */
  text-decoration: none;
}

/* Common */

aside,
nav,
footer,
header,
section,
main {
  display: block;
}

h1,
h2,
h3,
h4,
h5,
h6,
p {
  font-size: inherit;
  font-weight: inherit;
}

ul,
ul li {
  list-style: none;
}

img {
  vertical-align: top;
}

img,
svg {
  max-width: 100%;
  height: auto;
}

address {
  font-style: normal;
}

/* Form */

input,
textarea,
button,
select {
  font-family: inherit;
  font-size: inherit;
  color: inherit;
  background-color: transparent;
}

input::-ms-clear {
  display: none;
}

button,
input[type="submit"] {
  display: inline-block;
  box-shadow: none;
  background-color: transparent;
  background: none;
  cursor: pointer;
}

input:focus,
input:active,
button:focus,
button:active {
  outline: none;
}

button::-moz-focus-inner {
  padding: 0;
  border: 0;
}

label {
  cursor: pointer;
}

legend {
  display: block;
}

body {
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* 
nav {

  a {
    &.router-link-exact-active {
      color: #42b983;
    }
  }
} 
*/

h3 {
  font-size: 24px;
  margin: 10px 0;
}

#app {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  padding: 0 40px;
}

header {
  flex: 100%;
  // padding: 0 40px;

  nav {
    display: flex;
    padding: 20px 0;

    &:first-child {
      display: grid;
      grid-template-columns: 1fr 1fr auto auto;
      gap: 40px;

      div {
        margin: 0 auto 0 0;
      }

      svg {
        margin: 0 auto 0 0;
      }
    }

    &:last-child {
      display: flex;
      gap: 40px;

      button {
        margin: 0 auto 0 0;
      }

      form {
        margin: 0 0 0 auto;
      }
    }
  }
}

aside {
  flex: 0 1 20%;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

footer {
  align-items: center;
  background: #24292e;
  color: #fff;
  display: grid;
  flex: 100%;
  grid-template-columns: 400px 1fr;
  gap: 40px;
  padding: 80px 40px 40px;

  p {
    max-width: 600px;
  }

  div {
    display: flex;
    flex-direction: column;
    gap: 40px;

    .social {
      display: flex;
      gap: 20px;

      img {
        width: 30px;
      }

      // a {
      //   background: #53565a;
      //   border-radius: 50px;
      //   padding: 15px;
      // }
    }
  }

  .info {
    display: flex;
    gap: 20px;
    grid-area: 2;
    margin-top: 80px;
  }
}
</style>

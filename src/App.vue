<template>
  <header>
    <nav>
      <div></div>
      <img src="@/assets/logo.svg" width="200" alt="Ресторанный" />
      <button>Войти</button>
      <button>Регистрация</button>
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
    <article>
      <img src="@/assets/images/anita-austvika-mBVDi_cmkOg-unsplash.webp" alt="" />
      <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta
        eligendi placeat amet nulla quia et doloremque?
      </p>
    </article>

    <article>
      <img src="@/assets/images/anita-austvika-mBVDi_cmkOg-unsplash.webp" alt="" />
      <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta
        eligendi placeat amet nulla quia et doloremque?
      </p>
    </article>

    <article>
      <img src="@/assets/images/anita-austvika-mBVDi_cmkOg-unsplash.webp" alt="" />
      <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta
        eligendi placeat amet nulla quia et doloremque?
      </p>
    </article>

    <article>
      <img src="@/assets/images/anita-austvika-mBVDi_cmkOg-unsplash.webp" alt="" />
      <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta
        eligendi placeat amet nulla quia et doloremque?
      </p>
    </article>

    <article>
      <img src="@/assets/images/anita-austvika-mBVDi_cmkOg-unsplash.webp" alt="" />
      <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta
        eligendi placeat amet nulla quia et doloremque?
      </p>
    </article>

    <article>
      <img src="@/assets/images/anita-austvika-mBVDi_cmkOg-unsplash.webp" alt="" />
      <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores, soluta!</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias voluptatibus aperiam mollitia iusto sed doloribus dignissimos eaque deserunt! Nam perspiciatis accusamus molestias. Dicta
        eligendi placeat amet nulla quia et doloremque?
      </p>
    </article>
  </aside>

  <footer>
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus, temporibus nemo error suscipit ex dolore exercitationem iusto excepturi facilis veniam, quibusdam dolorem rem sint, amet
    distinctio in corrupti nihil incidunt.
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
}

header {
  flex: 100%;
  padding: 0 40px;

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

      img {
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
  flex: 100%;
  padding: 40px;
}
</style>

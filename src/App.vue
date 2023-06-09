<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class='logo'>
      <img alt="leandrocesar.com logo" class="logo" src="@/assets/logoBeta.svg" width="110" height="110" />
        <span class='logoAnimationSeven'>
          <h1 class='lightOnAnimationSeven'>leandrocesar.com</h1>
        </span>
        <span class='logoAnimationSevenTwo'>
          <h3>Consultoria & Serviços</h3>
        </span>
        <nav>
          <RouterLink to="/">INÍCIO</RouterLink>
          <RouterLink to="/projetos/ativos">PROJETOS</RouterLink>
          <RouterLink to="/sobre">SOBRE</RouterLink>
        </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
.logo{
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 2rem;
  color: hsla(160, 100%, 37%, 1);
}


h3{
  color: var(--color-text);
  margin-top: -1rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin: 2rem 0 ;
}

nav a {
  color: var(--color-text);
  font-weight: bold;
  font-size: .9rem;
}

nav a.router-link-exact-active {
  color: #00bd7e;
}

nav a.router-link-exact-active:hover {
  background-color: #00bd7e54;
  color: var(--color-text);
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

}
</style>

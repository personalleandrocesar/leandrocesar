<script setup lang="ts">
useHead({
    titleTemplate: 'leandrocesar.com',
})
</script>

<template>
  <header>
    <div class='logo'>
      <LCLogoFive/>
      <!-- <img alt="leandrocesar.com logo" class="logo" src="@/assets/logoBeta.svg" width="110" height="110" /> -->
        <span>
          <h1>leandrocesar.com</h1>
        </span>
        <span>
          <h3>Consultoria & Serviços</h3>
        </span>
        <nav>
          <NuxtLink to="/">CNPJ: 40.930.118/0001-33</NuxtLink>
        </nav>
    </div>
  </header>

</template>

<style scoped>
.logo{
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 2rem;
  color: #00DC82;
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
  color: #00DC82;
}

nav a.router-link-exact-active:hover {
  background-color: #00DC8254;
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
</style>

<template>
  <nav class="main-nav">
    <h2 class="logo" @click="$router.go(-1)">Vue App</h2>
    <nav class="links">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
  </nav>
  <router-view/>
</template>

<style lang="scss" src="./styles/reset.scss" />
<style lang="scss">
html {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.main-nav{
  height: 5rem;
  padding-inline: 1.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid #d5d5d5dd;
  box-shadow: #2c3e50 0 0 1px 0;

  .links {

    a {
      font-weight: bold;
      color: #2c3e50;

      &.router-link-exact-active {
        color: #42b983;
      }
    }
}

}
</style>

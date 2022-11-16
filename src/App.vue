<template>
  <nav>
    <h1>Inventory</h1>
    <router-link to="/">Home</router-link> |
    <router-link to="/book">Books</router-link> |
    <router-link to="/game">Game</router-link> |
    <router-link to="/gifts">Gifts</router-link> |
    <router-link to="/materials">Materials</router-link>
    <div class="topnav">
      <div class="search-container">
        <form action="/action_page.php">
          <input type="text" placeholder="Search.." name="search" >
          <button type="submit" >Search</button>
        </form>
      </div>
    </div>

  </nav>
  <div class="container text-start">
  <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1d2732;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>

<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <div class="wrapper">
      <p>JiwonSuh</p>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
  header {
    position: sticky;
    top: 0;
    left: 0;
    right: 0;
  }

  .wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1.4em;
  }

  a {
    text-decoration: none;
    color: var(--black);
  }
  
  a:hover {
    display: inline-block;
    border-bottom: 8px solid #EF5DA8;
    line-height: .8em;
  }

  hr {
    margin: 4em 0;
    border: 1px solid #c6c5c5a3;
  }
  
  .underline {
    display: inline-block;
    border-bottom: 8px solid #EF5DA8;
    line-height: .8em;
  }
</style>

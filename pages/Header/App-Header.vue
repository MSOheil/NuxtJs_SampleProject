<template>
  <ul>
    <h1>Header</h1>
    <li>
      <nuxt-link to="/">Home Page</nuxt-link>
    </li>
    <li>
      <nuxt-link to="/about">About</nuxt-link>
    </li>
    <li>
      <nuxt-link to="/jokes">Dad Jokes</nuxt-link>
    </li>
  </ul>
</template>
<script>

export default {
  name: 'AppHeader'
}
</script>

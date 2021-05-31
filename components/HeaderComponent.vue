<template>
  <div class="container">
    <div class="logo-and-search">
      <Logo />
      <FuzzySearch />
    </div>
    <div class="nav-links">
      <p>Pokemon</p>
      <p>Moves</p>
      <p>Map</p>
    </div>
  </div>
</template>

<script>
import Logo from '@/components/Logo.vue'
import FuzzySearch from '@/components/FuzzySearch.vue'

export default {
  components: {
    Logo,
    FuzzySearch,
  },
}
</script>

<style scoped>
.container {
  display: flex;
  height: 90px;
}

.container .logo-and-search {
  display: flex;
}

.nav-links {
  display: flex;
}
</style>

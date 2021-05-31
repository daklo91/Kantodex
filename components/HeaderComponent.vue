<template>
  <div class="container">
    <div class="logo-and-search">
      <Logo />
      <FuzzySearch class="fuzzy-search" />
    </div>
    <NavLinks class="nav-links" />
  </div>
</template>

<script>
import Logo from '@/components/Logo.vue'
import FuzzySearch from '@/components/FuzzySearch.vue'
import NavLinks from '@/components/NavLinks.vue'

export default {
  components: {
    Logo,
    FuzzySearch,
    NavLinks,
  },
}
</script>

<style scoped>
.container {
  display: flex;
  height: 90px;
  max-width: 1200px;
  margin: auto;
}

.container .logo-and-search {
  display: flex;
}

.container .logo-and-search .fuzzy-search {
  margin-left: 40px;
}

.nav-links {
  display: flex;
}
</style>

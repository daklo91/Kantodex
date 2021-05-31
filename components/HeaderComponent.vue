<template>
  <div class="shadow-container">
    <div class="container-header">
      <div class="logo-and-search">
        <Logo />
        <FuzzySearch class="fuzzy-search" />
      </div>
      <NavLinks class="nav-links" />
    </div>
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
.shadow-container {
  -webkit-box-shadow: 0px 1px 2px 0px rgba(0, 0, 0, 0.25);
  box-shadow: 0px 1px 2px 0px rgba(0, 0, 0, 0.25);
}

.container-header {
  display: flex;
  height: 90px;
  max-width: 1200px;
  margin: auto;
  margin-top: 10px;
  padding-left: 10px;
  flex-direction: row;
}

.logo-and-search {
  display: flex;
}

.fuzzy-search {
  margin-left: 40px;
}

.nav-links {
  display: flex;
  margin-right: 0;
}

@media screen and (max-width: 950px) {
  .container-header {
    flex-direction: column;
    height: 110px;
  }

  .logo-and-search {
    margin: auto;
  }

  .nav-links {
    margin: auto;
    margin-top: 10px;
    margin-bottom: 10px;
  }
}

@media screen and (max-width: 600px) {
  .container-header {
    height: 56px;
  }

  .nav-links {
    display: none;
  }

  .fuzzy-search {
    margin-left: 10px;
  }
}
</style>

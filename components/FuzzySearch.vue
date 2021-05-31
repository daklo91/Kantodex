<template>
  <div class="container">
    <input type="text" placeholder="Search" />
    <SearchIcon class="search-icon" />
  </div>
</template>

<script>
import SearchIcon from '@/components/SearchIcon.vue'

export default {
  components: {
    SearchIcon,
  },
}
</script>

<style scoped>
.container {
  background-color: var(--light-gray);
  border-radius: 8px;
  display: flex;
  max-height: 50px;
  margin: auto;
  margin-left: 40px;
  width: 225px;
  border: 2px solid transparent;
}

.container:focus-within {
  border: 2px solid var(--search-icon-blue);
}

.container input {
  background-color: var(--light-gray);
  height: 36px;
  margin: auto;
  border: 0px;
  font-size: 24px;
  width: 150px;
}

.container input:focus {
  outline: 0;
}

.container .search-icon {
  margin: auto;
}
</style>

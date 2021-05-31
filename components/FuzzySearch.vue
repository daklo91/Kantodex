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

input[type='text'] {
  font-family: var(--varela-round);
}

input::-webkit-input-placeholder {
  /* Chrome/Opera/Safari */
  font-family: var(--varela-round);
  color: var(--gray);
}
input::-moz-placeholder {
  /* Firefox 19+ */
  font-family: var(--varela-round);
  color: var(--gray);
}
input:-ms-input-placeholder {
  /* IE 10+ */
  font-family: var(--varela-round);
  color: var(--gray);
}
input:-moz-placeholder {
  /* Firefox 18- */
  font-family: var(--varela-round);
  color: var(--gray);
}

.container .search-icon {
  margin: auto;
}

@media screen and (max-width: 600px) {
  .container {
    max-height: 25px;
    width: 150px;
  }

  .container input {
    height: 20px;
    font-size: 18px;
    width: 100px;
  }
}
</style>

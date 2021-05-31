<template>
  <div class="container">
    <HeaderComponent />
    <h1>Header Above</h1>
  </div>
</template>

<script>
import HeaderComponent from '@/components/HeaderComponent.vue'
export default {
  components: {
    HeaderComponent,
  },
}
</script>

<style scope>
.container {
}
</style>

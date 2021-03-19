<template>
  <div class="error-container">
    error...
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'error'
    }
  }
}
</script>

<style scoped>
.error-container {
  height: 100vh;
  color: deeppink;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
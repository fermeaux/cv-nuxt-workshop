<template>
  <div class="container">
    {{ hello }}
  </div>
</template>

<script>
export default {
  data () {
    return { hello: 'world' }
  }
}
</script>

<style scoped>
.container {
  margin: 10rem;
}
</style>

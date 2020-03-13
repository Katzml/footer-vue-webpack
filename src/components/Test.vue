<template>
  <div>
      <h1 v-text="title"></h1>
  </div>
</template>

<script>
export default {
name:"Test",
props:{
    title: String
}
}
</script>

<style scoped>
    h1 {
        color: cyan;
        font-family: Arial, Helvetica, sans-serif;
    }
</style>
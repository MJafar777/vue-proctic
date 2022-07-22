<template>
  <div>
    <div class="card" v-for="comment in comments" v-bind:key="comment.id">
      <h2>Name :{{ comment.name }}</h2>
      <h2>Email :{{ comment.email }}</h2>
      <h2>Content :{{ comment.content }}</h2>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.card {
  border: 5px solid black;
  margin: 20px;
  box-sizing: border-box;
  padding: 10px;
}
</style>

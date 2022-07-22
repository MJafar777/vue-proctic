<template>
  <div>
    <h3>Add Comment</h3>
    <form @submit.prevent>
      <input
        type="text"
        v-bind:value="name"
        @input="name = $event.target.value"
        placeholder="Enter Your Name"
      />
      <input
        type="email"
        v-bind:value="email"
        @input="email = $event.target.value"
        placeholder="Enter Your Email"
      />
      <input
        type="text"
        v-bind:value="content"
        @input="content = $event.target.value"
        placeholder="Enter Your Content"
      />
      <button @click="createComment">Add Content</button>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style></style>

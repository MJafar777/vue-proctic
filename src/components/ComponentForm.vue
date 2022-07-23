<template>
  <div>
    <h3>Add Comment</h3>
    <form @submit.prevent>
      <input v-model="comment.name" placeholder="Enter Your Name" />
      <input v-model="comment.email" placeholder="Enter Your Email" />
      <input v-model="comment.content" placeholder="Enter Your Content" />
      <button @click="createComment">Add Content</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      comment: {
        name: "",
        email: "",
        content: "",
      },
    };
  },
};
</script>

<style></style>

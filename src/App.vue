<template>
  <div>
    <component-form />
    <component-list v-bind:comments="comments" />
  </div>
</template>

<script>
import ComponentForm from "./components/ComponentForm";
import ComponentList from "./components/ComponentList";

export default {
  components: {
    ComponentForm,
    ComponentList,
  },
  data() {
    return {
      comments: [
        {
          id: 1,
          name: "jafar",
          email: "jafar@gmail.com",
          content: "lorem ipsum ament",
        },
        {
          id: 2,
          name: "alex",
          email: "alex@gmail.com",
          content: "lorem ipsum ament",
        },
        {
          id: 3,
          name: "anna",
          email: "anna@gmail.com",
          content: "lorem ipsum ament",
        },
      ],
     
    };
  },
  methods: {
    createComment() {
      const newComments = {
        id: this.comments.length + 1,
        name: this.name,
        email: this.email,
        content: this.content,
      };
      this.comments.push(newComments);
      this.name = "";
      this.email = "";
      this.content = "";
    },
  },
};
</script>

<style></style>

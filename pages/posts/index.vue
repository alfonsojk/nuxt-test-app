<template>
  <div>
    <h1>Posts</h1>
    <Posts
      v-for="post of posts"
      :key="post.id"
      :id="post.id"
      :name="post.name"
    />
  </div>
</template>

<script>
import axios from "axios";
import Posts from "../../components/Post";
export default {
  components: {
    Posts
  },
  data() {
    return {
      posts: []
    };
  },
  async created() {
    const res = await axios.get(
      "https://jsonplaceholder.typicode.com/comments"
    );
    this.posts = res.data;
  }
};
</script>
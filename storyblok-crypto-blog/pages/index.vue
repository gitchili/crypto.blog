<template>
  <section class="container">
    <nuxt-link
      v-for="post in posts"
    :key="post.id"
    :to="post.id">
    <article class="post-preview">
      <div
     
      class="post-preview-thumbnail"></div>
      <div class="post-review-content"></div>
      <h1>{{ post.title }}</h1>
      <p>{{ post.previewText }}</p>
    </article>
    </nuxt-link>
 
    
  </section>
</template>

<script>

export default {
  data() {
    return {
      posts: [
        {
          title: "BlockChain News",
          previewText: 'Find the latest BlockChain.news',
          thumbnailUrl: "",
          id: "a-new-Beginning"
        },
        {
          title: "Crypto Tracker",
          previewText: 'Track crypto-assets',
          thumbnailUrl: "",
          id: "a-second-Beginning"
        }
      ]
    };
  }
};
</script>

<style>

</style>

<template>
  <section class="post-list">
      <PostPreview
        id='1'
        :is-admin='isAdmin'
        title="Hello"
        previewText='Hey There!'
        thumbnail='yellow'/>
      <PostPreview
        id='2'
        :is-admin='isAdmin'
        title="Hello"
        previewText='Hey There!'
        thumbnail='orange'/>
      <PostPreview
        id='3'
        :is-admin='isAdmin'
        title="Hello"
        previewText='Hey There!'
        thumbnail='green'/>
    </section>
</template>

<script>
import PostPreview from '@/components/posts/PostPreview.vue';

export default {
  components: {
    PostPreview,
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false,
    }
  }
};
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>

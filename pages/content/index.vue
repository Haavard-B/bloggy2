<template>
  <ContentPage title="Blog posts" :categories="categories" :selectedCategory="selectedCategory" />
</template>

<script>
export default {
  data() {
    return {
      selectedCategory: {name:"Select a topic", path: null},
      categories: [
        {name:"Essays", path: "blog/essays"},
        {name:"Research", path: "blog/research"}
      ],
    }
  },

  methods: {
  }
};
</script>

<style scoped>
</style>

<template>
  <ContentPage title="Blog posts" :categories="categories" :selectedCategory="selectedCategory" />
</template>

<script>
export default {
  data() {
    return {
      selectedCategory: {name:"Select a topic", path: null},
      categories: [
        {name:"checklists", path: "blog/checklists"},
        {name:"engineering", path: "blog/engineering"},
        {name:"philosophy", path: "blog/philosophy"},
      ],
    }
  },

  methods: {
  }
};
</script>

<style scoped>
</style>

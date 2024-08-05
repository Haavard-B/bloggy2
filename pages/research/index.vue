<template>
  <ContentPage title="Research" :selectedCategory="selectedCategory" />
</template>

<script>
export default {
  data() {
    return {
      selectedCategory: {name:"Research", path: "research"},
    }
  },

  methods: {
  }
};
</script>

<style scoped>
</style>

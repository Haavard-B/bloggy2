<template>
  <ContentPage title="Essays" :selectedCategory="selectedCategory" />
</template>

<script>
export default {
  data() {
    return {
      selectedCategory: {name:"Essays", path: "essays"},
    }
  },

  methods: {
  }
};
</script>

<style scoped>
</style>

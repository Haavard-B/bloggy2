<template>
  <div>
    <center class="mt-4">
      <TextTitle title="Hello" />
    </center>

    <MyCols :pages="pages" :cols="12" :xl="3" :lg="3" :md="12" :xs="12" v-slot="{ page }">
      <center>
        <nuxt-link :to="page.to">
          <v-btn text x-large color="blue darken-2" dark>{{ page.title }}</v-btn>
        </nuxt-link>

        <p class="grey--text">{{ page.description }}</p>
      </center>
    </MyCols>
  </div>
</template>


<script>
export default {
  data() {
    return {
      pages: [
        {
          title: "Read my notes",
          description: "They are not too messy",
          to: "/content",
        }
      ],
    };
  },
  mounted() {
    this.$router.push('/content');
  }
};
</script>

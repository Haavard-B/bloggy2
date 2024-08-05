<template>
  <div>
    <center class="mt-4">
      <TextTitle title="Hello" />

      <p class="mb-4">
        And I (still) have a <strong>plant</strong>
        <v-icon color="green" class="ml-0">mdi-flower</v-icon>
      </p>

      <MyHr class="my-12" />
    </center>

    <MyCols :pages="pages" :cols="12" :xl="3" :lg="3" :md="12" :xs="12" v-slot="{ page }">
      <center>
        <nuxt-link :to="page.to">
          <v-btn text x-large color="blue darken-2" dark>{{
            page.title
          }}</v-btn>
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
        },
        {
          title: "CV",
          description: "And other fun stuff",
          to: "/cv",
        },
        /* { */
        /*   title: "Consulting", */
        /*   description: "And what services I offer", */
        /*   to: "/consulting", */
        /* }, */
      ],
    };
  },
  mounted() {
    this.$router.push('/content');
  }
};
</script>

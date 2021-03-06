<template>
  <div>
    <h1>contact</h1>
    <button @click="redirect">redirect</button>
  </div>
</template>

<script>
export default {
  name: "Contact",
  methods: {
    redirect() {
      this.$router.push({
        path: "/",
      });
    },
  },
  mounted() {
    console.log(process.env.NUXT_ENV_TEST_ENV);
  },
};
</script>

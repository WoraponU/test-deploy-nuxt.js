<template>
  <div>
    <h1>Hello world!</h1>
    <button @click="redirect">redirect</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  methods: {
    redirect() {
      this.$router.push({
        path: "/contact",
      });
    },
  },
  mounted() {
    console.log(process.env.NUXT_ENV_TEST_ENV);
  },
};
</script>

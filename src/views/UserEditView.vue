<template>
  <div>Usuário {{ $route.params.id }}</div>
  <div>
    <button @click="login()">Login</button>
  </div>
</template>

<script>
export default {
  created() {
    // console.log(this.$router);
  },
  methods: {
    login() {
      this.$router.push({ name: "about" });
      console.log("ok");
    },
  },
};
</script>

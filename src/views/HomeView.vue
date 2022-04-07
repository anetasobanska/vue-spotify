<template>
  <div class="home">
    <h1>{{ name }}</h1>
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
  },
  data() {
    return {
      name: process.env.VUE_APP_NAME,
      clientId: process.env.VUE_APP_Client_ID,
      clientSecret: process.env.VUE_APP_Client_Secret,
    };
  },
};
</script>

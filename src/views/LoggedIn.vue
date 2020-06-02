<template>
  <div class="login">
    <loggedComp></loggedComp>
  </div>
</template>

<script>
import loggedComp from "@/components/loggedComp.vue";

export default {
  name: "Login",
  components: {
    loggedComp
  }
};
</script>

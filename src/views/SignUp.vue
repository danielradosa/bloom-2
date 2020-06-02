<template>
  <div class="login">
    <signupComp></signupComp>
  </div>
</template>

<script>
import signupComp from "@/components/signupComp.vue";

export default {
  name: "SignUp",
  components: {
    signupComp
  }
};
</script>

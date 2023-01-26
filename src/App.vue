<template>
  <h3>Hey!!!</h3>
  <Greeting></Greeting>
  <user :age="age"></user>
  <!-- note use of lowercase tags -->
</template>

<script>
import Greeting from "@/components/Greeting.vue";
import User from "@/components/User.vue";

export default {
  name: "App",
  components: {
    Greeting,
    User,
  },
  data() {
    return {
      age: 20,
    };
  },
};
</script>

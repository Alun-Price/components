<template>
  <h3>Hey!!!</h3>
  <button type="button" @click="age++">INCREASE AGE</button>
  <button type="button" @click="age--">DECREASE AGE</button>
  <Greeting :age="age"></Greeting>
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

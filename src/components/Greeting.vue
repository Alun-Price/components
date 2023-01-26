<template>
  <p v-if="age > 25">{{ msg }}</p>
  <p v-else>You must be 25 years or older to view this message</p>
</template>

<script>
export default {
  name: "Greeting",
  data() {
    return {
      msg: "Hello World!",
    };
  },
  props: ["age"],
};
</script>

<style scoped lang="scss">
p:hover {
  color: darken($color: #cc4444, $amount: 15%);
}
</style>

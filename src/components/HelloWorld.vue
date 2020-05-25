<template>
  <v-container>
    <v-btn dark x-large @click="spin=true" :loading="spin" block color="green">spin</v-btn>
    <v-btn dark x-large @click="spin=false"  block color="orange">Stop spin</v-btn>
  </v-container>
</template>

<script>
export default {
  name: "HelloWorld",

  data: () => ({
    spin: false
  })
};
</script>

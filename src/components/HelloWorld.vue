<template>
  <v-container>
    <v-img v-if="showImage" width="100" src="@/assets/images/image1.jpeg"></v-img>

    <v-btn dark x-large @click="showHideImage" block :color="color1">{{name}}</v-btn>
    
  </v-container>
</template>

<script>
export default {
  name: "HelloWorld",
  methods: {
    showHideImage() {
      if (this.showImage == true) {
        this.showImage = false;
        this.name="Show Image"
        this.color1="blue"
      } else {
        this.showImage = true;
        this.name="Hide Image"
        this.color1="orange"
      }
    }
 },
  data: () => ({
    color1: "blue",
    showImage: false,
    name: "Show Image"
  })
};
</script>

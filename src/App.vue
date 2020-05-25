<template>
  <v-app>
    <appMenu />
    <v-content>
      <HelloWorld />
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import appMenu from "./components/menu";
export default {
  name: "App",

  components: {
    HelloWorld,
    appMenu
  },

  data: () => ({
    //
  })
};
</script>

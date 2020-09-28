<template>
  <img alt="just logo" src="./assets/image-test.png" />
  <HelloWorld msg="Bonjour Le Coding en vue" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

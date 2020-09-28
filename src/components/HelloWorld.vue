<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">Page View count is: {{ count }}</button>
</template>

<script>
/*import { MDCTopAppBar } from '@material/top-app-bar';
const topAppBarElement = document.querySelector('.mdc-top-app-bar');
const topAppBar = new MDCTopAppBar(topAppBarElement);*/

export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      count: 0,
    };
  },
};


</script>

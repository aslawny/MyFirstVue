<template>
  <header>
    <div class="wrap">
      <div id="hamburger" v-on:click="display_menu()">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <nav id="menu">
        <li><a>Menu 1</a></li>
        <li class="drop">
          <a v-on:click="display_drop_menu()"
            >Menu 2 dropdown <i class="icon-arrow"></i
          ></a>
          <ul class="drop_menu">
            <a>Sub menu 1</a>
            <a>Sub menu 2</a>
            <a>Sub menu 3</a>
          </ul>
        </li>
        <li class="drop">
          <a v-on:click="display_drop_menu()"
            >Menu 3 dropdown <i class="icon-arrow"></i
          ></a>
          <ul class="drop_menu">
            <a>Sub menu 1</a>
            <a>Sub menu 2</a>
            <a>Sub menu 3</a>
          </ul>
        </li>
        <li><a>Menu 4</a></li>
      </nav>
    </div>
  </header>
  <div id="loader" v-if="load">
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
  </div>
  <div id="overlay" v-if="load"></div>
  <div id="background">
    <h3>This menu is responsive, resized on.</h3>
    <h3>
      The header is hide when scroll down and show when scroll up, try it !
    </h3>
    <button v-on:click="loaded()">Click here for loader!</button>
  </div>
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

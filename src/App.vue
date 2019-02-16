<template>
  <div id="app">
    <app-nav></app-nav>
    <router-view class="container"/>
  </div>
</template>

<script>
import AppNav from "@/components/AppNav";

export default {
  components: {
    AppNav
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Merriweather+Sans");

#app {
  font-family: "Merriweather Sans", sans-serif;
}
</style>

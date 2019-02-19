<template>
  <div class="home">
    <div class="jumbotron mt-4">
      <h1 class="display-3">Welcome to Community!</h1>
      <p class="lead">A fully open source forum. Built with Node, Express, Postgres And Vue!</p>
      <hr class="my-4">
      <p></p>
      <p class="lead mt-4">
        <a class="btn btn-primary btn-lg" :href="getLoginURL" role="button">Login with Google</a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  methods: {},
  computed: {
    getLoginURL() {
      if (window.location.hostname === "localhost") {
        return "http://localhost:3000/auth/google";
      } else {
        return "https://forum-community.herokuapp.com/auth/google";
      }
    }
  }
};
</script>

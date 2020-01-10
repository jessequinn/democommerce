<template>
  <section class="hero">
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title is-spaced">
          The New PiperNet
        </h1>
        <h2 class="subtitle">
          Decentralized, secure, private. The PiperNet
          <Fas i="theater-masks"/> is on it's way to revolutionize every smartphone and PC near you.
        </h2>
        <a class="button is-centered is-primary" href="#">Sign up for free</a>
        <a class="button is-centered is-light" href="#">Read more</a>
      </div>
    </div>
  </section>
</template>

<script>
  import Fas from "./Fas";

  export default {
    name: "AppBanner", components: {
      Fas
    }
  }
</script>

<style scoped>

</style>

<template>
  <section id="about" class="section">
    <div class="container has-text-centered">
      <div class="image avatar">
        <img src="../assets/img/profile-2.jpg">
      </div>
      <h2 class="title is-2">About</h2>
      <separator></separator>
      <div class="about-text block">
        I am Arul, FullStack Developer from Makassar.
        <br>
        Since I was little, I was interested in computers and made things and this has led me to the world of the internet as a developer who creates all kinds of things!
        <br>
        Currently a freelance web developer, in Jakarta. I have completed the Bachelor of Information Systems Program at STMIK Dipanegara Makassar.
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "about",
  data() {
    return {};
  },
  mounted() {
    sr.reveal("#about .block", 200);
  }
};
</script>

<style lang="scss" scoped>
@import "~vars";

.avatar {
  height: 200px;
  width: 200px;
  margin: 1rem auto;

  img {
    user-select: none;
    pointer-events: none;
    border-radius: 200px;
    border: 3px solid $secondary;
  }
}

.about-text {
  max-width: $tablet;
  margin: auto;
}
</style>

<template>
  <footer class="footer">
    <div class="container">
      <div class="content has-text-centered">
        <p class="reveal">
          © 2018 djaduls, made with lots of ❤️ and steaming hot ☕️.
        </p>
        <p class="reveal">
          <a class="icon"
            v-for="item in social"
            :href="item.link"
            :key="item.id"
            target="_blank"
            rel="noopener">
            <b-icon :icon="item.icon"></b-icon>
          </a>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "copyright",
  mounted() {
    sr.reveal(".footer .reveal", 250);
  },
  data() {
    return {
      social: [
        {
          icon: "facebook",
          link: "https://www.facebook.com/djaduls"
        },
        {
          icon: "instagram",
          link: "https://www.instagram.com/djaduls"
        },
        {
          icon: "linkedin",
          link: "https://www.linkedin.com/in/khairul-baharuddin-924831107"
        },
        {
          icon: "twitter",
          link: "https://twitter.com/djaduls"
        },
        {
          icon: "google-plus",
          link: "https://plus.google.com/+aruldjaduls"
        },
        {
          icon: "github",
          link: "https://github.com/arul21"
        },
        
      ]
    };
  }
};
</script>

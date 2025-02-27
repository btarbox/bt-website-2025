<template>
  <div class="dizme_tm_header">
    <div class="container">
      <div class="inner">
        <div class="logo">
          <a href="#" class="logoText">
            Brian Tarbox
          </a>
        </div>
        <div class="menu">
          <ul class="anchor_nav">
            <li class="current"><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#service">Service</a></li>

            <!-- <li><a href="#contact">Contact</a></li> -->
            <li class="download_cv">
              <a @click="openLinkedInProfile"><span>Connect on LinkedIn</span></a>
            </li>
            <!-- <li class="download_cv">
              <a href="img/cv/1.jpg" download><span>Download CV</span></a>
            </li> -->
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderVue",
  props: {
    dark: { type: Boolean },
  },
  methods: {
    openLinkedInProfile() {
      let url = 'https://www.linkedin.com/in/briantarbox/';
      let newWindow = window.open(url, '_blank', 'noreferrer,noopener');
      if (newWindow) newWindow.opener = null;
    }
  }
};
</script>

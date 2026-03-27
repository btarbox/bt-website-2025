<template>
  <PreLoader />
  <router-view />
  <Cursor />
</template>

<script>
import Cursor from "./components/layout/Cursor.vue";
import PreLoader from "./components/layout/PreLoader.vue";
import {
  dataImage,
  portfolioHover,
  scroll_,
  stickyNav,
  wowJsAnimation,
} from "./utils";

export default {
  name: "App",
  data() {
    return { dark: false };
  },
  mounted() {
    wowJsAnimation();
    window.addEventListener("scroll", stickyNav);
    window.addEventListener("scroll", scroll_);
    setTimeout(() => {
      dataImage();
      portfolioHover();
    }, 100);
  },
  components: { PreLoader, Cursor },
};
</script>

<style>
/* --- TOOLTIP STYLES START --- */
.tooltip-link {
    position: relative;
    display: inline-block;
    cursor: pointer;
}

.tooltip-link::after {
    content: attr(data-tooltip);
    position: absolute;
    bottom: 125%;
    left: 50%;
    transform: translateX(-50%) translateY(10px);
    background-color: #333;
    color: #fff;
    padding: 8px 12px;
    border-radius: 6px;
    font-size: 14px;
    white-space: nowrap;
    opacity: 0;
    pointer-events: none;
    transition: all 0.3s ease;
    z-index: 9999 !important;
}

.tooltip-link:hover::after {
    display: inline-block !important;
    position: relative;
    opacity: 1;
    transform: translateX(-50%) translateY(0);
}
/* --- TOOLTIP STYLES END --- */
</style>

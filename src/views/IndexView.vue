<template>
  <div class="dizme_tm_all_wrap" data-magic-cursor="show">
    <MobileHeaderVue />
    <HeaderVue />
    <HomeComponent />
    <!-- HERO -->

    <!-- PROCESS -->
    <ProcessComponent />
    <!-- /PROCESS -->

    <!-- ABOUT -->
    <AboutComponent />
    <!-- /ABOUT -->

    <!-- PORTFOLIO -->
    <PortfolioComponent />
    <!-- /PORTFOLIO -->

    <!-- SKILLS -->
    <SkillComponent />
    <!-- /SKILLS -->

    <!-- SERVICES -->
    <ServiceCompoent />
    <!-- /SERVICES -->

    <!-- TESTIMONIALS -->
    <TestimonialsComponent />
    <!-- /TESTIMONIALS -->

    <!-- PARTNERS -->
    <PartnersComponent />
    <!-- /PARTNERS -->

    <!-- NEWS -->
    <!-- NewsComponent /> -->
    <!-- /NEWS -->

    <!-- SUBSCRIBE -->
    <SubscribeComponent />
    <!-- /SUBSCRIBE -->

    <!-- CONTACT -->
    <ContactComponent />
    <!-- /CONTACT -->

    <!-- COPYRIGHT -->
    <CopyrightComponent />
    <!-- /COPYRIGHT -->

    <ScrollTopVue />
  </div>
</template>

<script>
import HeaderVue from "@/components/layout/Header.vue";
import MobileHeaderVue from "@/components/layout/MobileHeader.vue";
import ScrollTopVue from "@/components/layout/ScrollTop.vue";
import { activeSkillProgress } from "@/utils";
import AboutComponent from "../components/AboutComponent.vue";

import CopyrightComponent from "../components/CopyrightComponent.vue";
import HomeComponent from "../components/HomeComponent.vue";


import PortfolioComponent from "../components/PortfolioComponent.vue";
import ProcessComponent from "../components/ProcessComponent.vue";
import ServiceCompoent from "../components/ServiceCompoent.vue";
import SkillComponent from "../components/SkillComponent.vue";

import TestimonialsComponent from "../components/TestimonialsComponent.vue";

export default {
  name: "IndexView",
  components: {
    HomeComponent,
    ProcessComponent,
    AboutComponent,
    PortfolioComponent,
    SkillComponent,
    ServiceCompoent,
    TestimonialsComponent,



    CopyrightComponent,
   
    HeaderVue,
    MobileHeaderVue,
    ScrollTopVue,
  },
  mounted() {
    window.addEventListener("scroll", activeSkillProgress);
  },
};
</script>

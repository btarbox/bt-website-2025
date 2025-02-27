<template>
  <div class="dizme_tm_section" id="home">
    <div class="dizme_tm_hero">
      <div
        class="background"
        :data-img-url="`/img/slider/${dark ? 2 : 1}.jpg`"
      ></div>
      <div class="container">
        <div class="content">
          <div class="details">
            <div class="hello">
              <h3 class="orangeText">Hello, I'm</h3>
            </div>
            <div class="name">
              <h3>Brian Tarbox</h3>
            </div>
            <div class="job">
              <p>
                Experienced <span class="orangeText">Software Developer</span> and
                <span class="orangeText">AWS Expert</span>
              </p>
            </div>
            <div class="text">
              <p>
                Based in the ever-evolving world of technology, I have dedicated four decades to mastering my craft in software development. With a particular passion for Amazon Web Services (AWS), I have spent the last decade immersing myself in this domain, becoming a recognized authority in architecting and implementing cloud solutions.
              </p>
            </div>
            <div class="button">
              <div class="dizme_tm_button">
                <a class="anchor" href="#about"><span>About Me</span></a>
              </div>
              <div class="social">
                <ul>
                  <li>
                    <a href="#"><i class="icon-facebook-1"></i></a>
                  </li>
                  <li>
                    <a href="#"><i class="icon-twitter-1"></i></a>
                  </li>
                  <li>
                    <a href="#"><i class="icon-linkedin-1"></i></a>
                  </li>
                  <li>
                    <a href="#"><i class="icon-behance"></i></a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div class="avatar">
            <div class="image">
              <!-- <img src="/img/slider/avatar.png" alt="" width="390px"
                height="390px" /> -->
              <img 
                class="profilePictureHero"
                src="/img/slider/profile.png" 
                alt=""
              />
              <img
                class="skills illustrator anim_moveBottom"
                src='/img/badges/AlexaChampions.png' alt=""/>
              <img 
                class="skills photoshop anim_moveBottom" 
                src='/img/badges/AWSHeroes.png'/>
              <img 
                class="skills figma anim_moveBottom" 
                src='/img/badges/Usergroups-badges_leader-dark.png'/>
            </div>
          </div>
        </div>
      </div>
      <div class="dizme_tm_down">
        <a class="anchor" href="#process" v-html="dark ? mouseDark : mouse">
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import { figma, mouse, mouseDark, ps } from "../svg";
export default {
  name: "HomeComponent",
  data() {
    return { 
      ps, figma, mouse, mouseDark,
      AlexaChampion: '/img/badges/AlexaChampions.png',
    };
  },
  props: {
    dark: { type: Boolean },
  },
};
</script>

<template>
  <div class="dizme_tm_section">
    <div class="dizme_tm_skills">
      <div class="container">
        <div class="wrapper">
          <div class="left">
            <div
              class="dizme_tm_main_title wow fadeInUp"
              data-wow-duration="1s"
              data-align="left"
            >
              <span>Building and Transforming</span>
              <h3>I Continually Enhance My Knowledge to Stay at the Forefront of Innovation</h3>
              <p>
                Embracing an ever-evolving landscape, I consistently refine my skills to stay abreast of the latest advancements in software development and cloud solutions.
              </p>
            </div>
            <div class="dodo_progress wow fadeInUp" data-wow-duration="1s">
              <div
                class="progress_inner skillsInner___"
                data-value="85"
                data-color="#f75023"
              >
                <span
                  ><span class="label">AWS Architecture</span
                  ><span class="number">90%</span></span
                >
                <div class="background">
                  <div class="bar"><div class="bar_in"></div></div>
                </div>
              </div>
              <div
                class="progress_inner skillsInner___"
                data-value="95"
                data-color="#1cbe59"
              >
                <span
                  ><span class="label">Diversity Advocacy</span
                  ><span class="number">95%</span></span
                >
                <div class="background">
                  <div class="bar"><div class="bar_in"></div></div>
                </div>
              </div>
              <div
                class="progress_inner skillsInner___"
                data-value="75"
                data-color="#8067f0"
              >
                <span
                  ><span class="label">Mentorship & Education</span
                  ><span class="number">85%</span></span
                >
                <div class="background">
                  <div class="bar"><div class="bar_in"></div></div>
                </div>
              </div>
            </div>
          </div>
          <div class="right">
            <img :src="`/img/skills/${dark ? 2 : 1}.jpg`" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SkillComponent",
  components: {},
  props: {
    dark: { type: Boolean },
  },
};
</script>

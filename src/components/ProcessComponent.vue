<template>
  <div class="dizme_tm_section" id="process">
    <div class="dizme_tm_process">
      <div class="container">
        <div class="list">
          <ul>
            <li class="wow fadeInUp" data-wow-duration="1s">
              <div class="list_inner">
                <div class="icon">
                  <span v-html="dark ? pixelPerfectDark : pixelPerfectLight">
                  </span>
                </div>
                <div class="title">
                  <h3>Cloud Solutions Architect</h3>
                </div>
                <div class="text">
                  <p>
                    Tap into my decades-long experience with AWS, cloud, and infrastructure as I help create robust and scalable cloud solutions tailored to your most-wished business needs and desired technical outcomes.
                  </p>
                </div>
              </div>
            </li>
            <li
              class="wow fadeInUp"
              data-wow-duration="1s"
              data-wow-delay="0.2s"
            >
              <div class="list_inner">
                <div class="icon">
                  <span v-html="dark ? awesomeIdeaDark : awesomeIdeaLight">
                  </span>
                </div>
                <div class="title">
                  <h3>Diversity/Inclusion Advocate</h3>
                </div>
                <div class="text">
                  <p>
                    Harness the power of diversity and inclusion in your organization. I'll work alongside you to foster an inclusive tech environment, championing equal opportunities and empowering underrepresented groups.
                    <br/><br/> In 2021 58% of the speakers at the User Group I organize were not white men.
                  </p>
                </div>
              </div>
            </li>
            <li
              class="wow fadeInUp"
              data-wow-duration="1s"
              data-wow-delay="0.4s"
            >
              <div class="list_inner">
                <div class="icon">
                  <span v-html="dark ? highQualityDark : highQualityLight">
                  
                  </span>
                </div>
                <div class="title">
                  <h3>Experienced Mentor</h3>
                </div>
                <div class="text">
                  <p>
                    Leverage my 40 years of programming knowledge for your team's development. Through impactful workshops, speaking engagements, and  articles, I can guide growth through evolving tech landscapes.
                  <br/><br/>
                  I was one of the initial Hero Mentors in the AWS New Voices program.  We taught Community Builders how to structure and present technical talks.                  </p>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import {
  awesomeIdeaDark,
  awesomeIdeaLight,
  highQualityDark,
  highQualityLight,
  pixelPerfectDark,
  pixelPerfectLight,
} from "@/svg";
export default {
  name: "ProcessComponent",
  data() {
    return {
      pixelPerfectLight,
      highQualityDark,
      awesomeIdeaDark,
      pixelPerfectDark,
      awesomeIdeaLight,
      highQualityLight,
    };
  },
  components: {},
  props: {
    dark: { type: Boolean },
  },
};
</script>

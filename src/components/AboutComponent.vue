<template>
  <div class="dizme_tm_section" id="about">
    <div class="dizme_tm_about">
      <div class="container">
        <div class="wrapper">
          <div class="left">
            <div class="image">
              <img :src="`/img/about/${dark ? 2 : 1}.jpg`" alt="" />
              <div class="numbers year">
                <div class="wrapper">
                  <h3>
                    <!-- <VueJsCounter end="40"></VueJsCounter> -->
                    40
                  </h3>
                  <span class="name">Years of<br />Success</span>
                </div>
              </div>
              <div class="numbers project">
                <div class="wrapper">
                  <h3 style="display: flex">
                    <!-- <VueJsCounter as="span" end="100"></VueJsCounter>s -->
                    100
                  </h3>
                  <span class="name">Of Total<br />Projects</span>
                </div>
              </div>
            </div>
          </div>
          <div class="right">
            <div class="title wow fadeInUp" data-wow-duration="1s">
              <span>I'm a Builder</span>
              <h3>I Craft Powerful Cloud Infrastructure and Promote Tech Inclusivity</h3>
            </div>
            <div class="text wow fadeInUp" data-wow-duration="1s">
              <p>
                Brian Tarbox is a highly experienced and accomplished software developer with a remarkable programming journey spanning a long time. With a strong foundation built over 40 years of coding expertise, including a decade dedicated to Amazon Web Services (AWS), Brian has honed his skills and become a recognized authority in the field. His deep knowledge and proficiency in AWS services have made him a valuable asset in architecting and implementing cloud solutions.
                <br/><br/>
                Brian has a Master's degree in Cognitive Pyschology from the University of Hawaii at Manoa where he studied "language" learning in bottlenosed Dolphins.
                <br/><br/>
                He also has BA from Wesleyan University in Linguistic Philosophy.
                <br/><br/>
                Beyond his technical prowess, Brian has embraced a profound commitment to diversity, inclusion, and giving back to the community. With a genuine passion for fostering an inclusive tech industry, he actively advocates for equal opportunities and the empowerment of underrepresented groups. Brian's dedication to these principles is evident in his numerous initiatives, where he champions diversity and strives to create a welcoming environment for all.
                <br/>
                <br/>
                As a mentor and educator, Brian shares his wealth of knowledge with aspiring developers, delivering impactful workshops, speaking engagements, and authoring insightful articles. His ability to inspire others and provide guidance in their coding journeys has made him a sought-after resource within the industry.
                <br/>
                <br/>
                With a strong sense of purpose and an unwavering focus on making a positive impact, Brian Tarbox combines his extensive technical background with his deep-rooted values of diversity, inclusion, and community support. His personal website serves as a platform to share his expertise, engage with fellow professionals, and contribute to the ongoing dialogue surrounding these critical topics. Through his leadership, Brian continues to drive positive change, leaving a lasting legacy in the technology landscape.
              </p>
            </div>
            <div class="dizme_tm_button wow fadeInUp" data-wow-duration="1s">
            </div>
          </div>
        </div>
      </div>
      <div class="brush_1 wow fadeInLeft" data-wow-duration="1s">
        <img src="/img/brushes/about/1.png" alt="" />
      </div>
      <div class="brush_2 wow fadeInRight" data-wow-duration="1s">
        <img src="/img/brushes/about/2.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
// import VueJsCounter from "vue-js-counter";
export default {
  name: "AboutComponent",
  // components: { VueJsCounter },
  props: {
    dark: { type: Boolean },
  },
};
</script>

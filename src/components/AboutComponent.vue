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
                <br/><br/>
Brian Tarbox has been writing software for 40 years, the last decade of it focused on AWS. He's an AWS Community Hero, AWS Ambassador, and Alexa Champion, and works today as a Principal Solutions Architect helping companies design and build cloud systems that hold up in production.
                <br/><br/>
His background isn't the usual path into tech. Brian holds a Master's in Cognitive Psychology from the University of Hawai'i at Mānoa, where he studied language learning in bottlenose dolphins, and a BA in Linguistic Philosophy from Wesleyan University. That combination, the study of how minds and language actually work, shapes how he thinks about systems, communication, and now AI: he's currently applying Gricean pragmatics to how large language models handle ambiguity.

                <br/><br/>
Outside of architecture work, Brian leads Caylent's Neurodiversity Employee Resource Group and mentors underrepresented engineers through the AWS New Voices program. He speaks regularly at conferences, writes technical articles, and holds ten US patents. He's also a private pilot, rescue scuba diver, and musician who's spent a fair amount of time turning AWS telemetry into music (ask him about the CloudWatch Sonifier sometime).
                <br/>
This site is where he writes about all of it: cloud architecture, AI, cognitive science, and the occasional dolphin.
                <br/>
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

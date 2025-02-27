<template>
  <div class="dizme_tm_section">
    <div class="dizme_tm_testimonials">
      <div class="dizme_tm_main_title" data-align="center">
        <span>Testimonials</span>
        <h3>What My Clients & Colleagues Say</h3>
        <p>
          Hear directly from those who've benefited from my expertise in AWS solutions, commitment to diversity advocacy, and nurturing mentorship.
        </p>
      </div>
      <div class="list_wrapper">
        <div class="total">
          <div class="in">
            <swiper
              :pagination="{ clickable: true, el: '.owl-dots' }"
              :modules="modules"
              class="owl-carousel owl-theme"
            >
              <swiper-slide>
                <div class="icon" v-html="testimonialIcon"></div>
                <div class="text">
                  <p>
                    Brian joined Foundation Medicine on the CloudOps team as a Cloud Architect. I had known Brian from the Boston-area AWS professionals group, and his knowledge of all things AWS was astounding and felt like a great fit. He definitely can speak AWS and do as he says. His ability to adapt to change, which is a constant in architecture these days as technology advances, is unparalleled. He's professional but also has a sharp wit that works well with me as a colleague.
                  </p>
                </div>
                <div class="short">
                  <div class="image">
                    <img
                      class="main"
                      src="/img/testimonials/eric-haberman.jpeg"
                    />
                  </div>
                  <div class="detail">
                    <h3>Erich Haberman</h3>
                    <span>Architect II, Foundation Medicine</span>
                  </div>
                </div>
              </swiper-slide>
              <swiper-slide>
                <div class="icon" v-html="testimonialIcon"></div>
                <div class="text">
                  <p>
                    As the owner of the AWS Developer Podcast, I had the pleasure of interviewing Brian directly, and I can attest to his exceptional qualities. He is not only knowledgeable, but he also possesses an extraordinary talent for communicating difficult concepts with ease, which is a rare and valuable skill. I highly recommend Brian for any role or project that requires a kindhearted, intelligent, and dedicated individual. He is truly a remarkable person who has the potential to make a significant positive impact on any team or organization.
                  </p>
                </div>
                <div class="short">
                  <div class="image">
                    <img
                      class="main"
                      src="/img/testimonials/dave-isbitski.jpeg"
                    />
                  </div>
                  <div class="detail">
                    <h3>Dave Isbitski</h3>
                    <span>Principal Developer Advocate, Amazon Web Services</span>
                  </div>
                </div>
              </swiper-slide>
              <swiper-slide>
                <div class="icon" v-html="testimonialIcon"></div>
                <div class="text">
                  <p>
                    Brian joined my cloud team as a one of the first Architects into a newly formed 
                    practice, as a direct report. Said simply, his in-depth knowledge of AWS services 
                    and functions is incredible. Brian is an active AWS Community Hero, speaker, and 
                    participant, who can talk the talk but also get in and do the work. Yet, Brian 
                    carries with him a uniqueness in the realm of architecture – he is thoughtful, 
                    communicative, and inclusive. He has led the charge at FMI on moving from 
                    CloudFormation to Terraform, helping to train our engineers and devops staff. 
                    He’s been instrumental in helping to define MVP state of many global initiatives 
                    at scale within the organization and can recognize gaps, document reason, and 
                    present viable solutions. Brian’s thoughtfulness leads the way in the work he does 
                    as a valued member of the team.
                  </p>
                </div>
                <div class="short">
                  <div class="image">
                    <img
                      class="main"
                      src="/img/testimonials/daniel-gerow.jpeg"
                    />
                  </div>
                  <div class="detail">
                    <h3>Daniel Gerow</h3>
                    <span>VP Cloud Platform & Production Engineering, Collibra</span>
                  </div>
                </div>
              </swiper-slide>
            </swiper>
            <div class="owl-dots"></div>
          </div>
          <div class="left_details">
            <!-- <div
              class="det_image one wow fadeIn"
              data-wow-duration="1s"
              data-img-url="/img/testimonials/2.jpg"
            ></div>
            <div
              class="det_image two wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.2s"
              data-img-url="/img/testimonials/1.jpg"
            ></div>
            <div
              class="det_image three wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.4s"
              data-img-url="/img/testimonials/3.jpg"
            ></div>
            <div
              class="det_image four wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.6s"
              data-img-url="/img/testimonials/4.jpg"
            ></div> -->
            <!-- <span class="circle green animPulse"></span>
            <span class="circle yellow animPulse"></span>
            <span class="circle border animPulse"></span> -->
          </div>
          <div class="right_details">
            <!-- <div
              class="det_image one wow fadeIn"
              data-wow-duration="1s"
              data-img-url="/img/testimonials/5.jpg"
            ></div>
            <div
              class="det_image two wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.2s"
              data-img-url="/img/testimonials/6.jpg"
            ></div>
            <div
              class="det_image three wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.4s"
              data-img-url="/img/testimonials/7.jpg"
            ></div> -->
            <!-- <span class="circle yellow animPulse"></span>
            <span class="circle purple animPulse"></span>
            <span class="circle border animPulse"></span> -->
          </div>
        </div>
      </div>
      <div class="brush_1 wow fadeInRight" data-wow-duration="1s">
        <img src="/img/brushes/testimonials/1.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import { testimonialIcon } from "@/svg";
import { Pagination } from "swiper";
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
export default {
  name: "TestimonialsComponent",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      testimonialIcon,
    };
  },
  setup() {
    return {
      modules: [Pagination],
    };
  },
};
</script>

<template>
  <div class="dizme_tm_section" id="contact">
    <div class="dizme_tm_contact">
      <div class="container">
        <div class="dizme_tm_main_title" data-align="center">
          <span>Contact Me</span>
          <h3>I Want To Hear From You</h3>
          <p>
            Please fill out the form on this section to contact with me. Or call
            between 9:00 a.m. and 8:00 p.m. ET, Monday through Friday
          </p>
        </div>
        <div class="contact_inner">
          <div class="left wow fadeInLeft" data-wow-duration="1s">
            <ul>
              <li>
                <div class="list_inner">
                  <div class="icon orangeBackground">
                    <i class="icon-location orangeText"></i>
                  </div>
                  <div class="short">
                    <h3>Address</h3>
                    <span>Littleton, MA (outside of Boston)</span>
                  </div>
                </div>
              </li>
              <li>
                <div class="list_inner">
                  <div class="icon greenBackground">
                    <i class="icon-mail-1 greenText"></i>
                  </div>
                  <div class="short">
                    <h3>Email</h3>
                    <span><a href="#">BrianTarbox@gmail.com</a></span>
                  </div>
                </div>
              </li>
              <li>
                <div class="list_inner">
                  <div class="icon purpleBackground">
                    <i class="icon-phone purpleText"></i>
                  </div>

                </div>
              </li>
            </ul>
          </div>
          <div class="right wow fadeInRight" data-wow-duration="1s">
            <div class="fields">
              <form
                action="/"
                method="post"
                class="contact_form"
                id="contact_form"
                autocomplete="off"
              >
                <div
                  class="returnmessage"
                  data-success="Your message has been received, We will contact you soon."
                ></div>
                <div class="empty_notice">
                  <span>Please Fill Required Fields</span>
                </div>
                <div class="input_list">
                  <ul>
                    <li>
                      <input id="name" type="text" placeholder="Your Name" />
                    </li>
                    <li>
                      <input id="email" type="text" placeholder="Your Email" />
                    </li>
                    <li>
                      <input
                        id="phone"
                        type="number"
                        placeholder="Your Phone"
                      />
                    </li>
                    <li>
                      <input id="subject" type="text" placeholder="Subject" />
                    </li>
                  </ul>
                </div>
                <div class="message_area">
                  <textarea
                    id="message"
                    placeholder="Write your message here"
                  ></textarea>
                </div>
                <div class="dizme_tm_button">
                  <a id="send_message" href="#"><span>Submit Now</span></a>
                </div>
              </form>
            </div>
          </div>
          <div class="brush_2 wow fadeInRight" data-wow-duration="1s">
            <img src="img/brushes/contact/2.png" alt="" />
          </div>
        </div>
      </div>
      <div class="brush_1 wow fadeInLeft" data-wow-duration="1s">
        <img src="img/brushes/contact/1.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactComponent",
  components: {},
};
</script>

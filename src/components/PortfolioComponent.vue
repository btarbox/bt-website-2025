<template>
  <div class="dizme_tm_section" id="portfolio">
    <div class="dizme_tm_portfolio">
      <div class="container">
        <div class="dizme_tm_main_title" data-align="center">
          <span>Portfolio</span>
          <h3>Impactful Initiatives and Solutions</h3>
          <p>
            Explore a range of my significant contributions in cloud computing and innovation, demonstrating a blend of technical acumen and commitment to inclusive practices in technology.
          </p>
        </div>
        <div class="portfolio_filter">
          <ul>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '1' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '1')"
                data-filter="*"
                >All</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '2' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '2')"
                data-filter=".alexa"
                >Alexa Skills</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '3' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '3')"
                data-filter=".awards"
                >Awards</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '4' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '4')"
                data-filter=".BAWSton"
                >BAWSton User Group</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '11' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '4')"
                data-filter=".Certifications"
                >Certifications</a
              >
            </li>            <li>
              <a
                class="c-pointer"
                :class="activeNav === '5' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '5')"
                data-filter=".Dolphins"
                >Dolphins</a
              >
            </li>

            <li>
              <a
                class="c-pointer"
                :class="activeNav === '7' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '7')"
                data-filter=".OriginalMusic"
                >Original Music</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '8' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '8')"
                data-filter=".Patents"
                >Patents</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '9' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '9')"
                data-filter=".Presentations"
                >Presentations</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '10' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '10')"
                data-filter=".Publications"
                >Publications</a
              >
            </li>

            
          </ul>
        </div>
        <div class="dizme_tm_portfolio_titles"></div>
        <div class="portfolio_list wow fadeInUp" data-wow-duration="1s">
          <ul class="gallery_zoom grid">
            
            <li class="alexa grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Alexa Skills"
                  data-category="Alexa"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 2"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/Alexa/alexa-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Alexa Skills</h3>
                  <span>Alexa</span>
                </div>
              </div>
            </li>

            <li class="awards grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Awards & Accolades"
                  data-category="Awards"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 3"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/Awards/awards-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Awards & Accolades</h3>
                  <span>Awards</span>
                </div>
              </div>
            </li>

            <li class="BAWSton grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="BAWSton"
                  data-category="BAWSton"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 4"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/BAWSton/bawston-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>BAWSton User Group</h3>
                  <span>AWS User Group</span>
                </div>
              </div>
            </li>


            <li class="Certifications grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Certifications"
                  data-category="Certifications"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 11"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/certifications.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Certifications</h3>
                  <span>ACertifications</span>
                </div>
              </div>
            </li>

            <li class="Dolphins grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Dolphins"
                  data-category="Dolphins"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 5"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/Dolphins/dolphins-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Dolphins</h3>
                  <span>Dolphins</span>
                </div>
              </div>
            </li>



            <li class="OriginalMusic grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Awards & Accolades"
                  data-category="OriginalMusic"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 7"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/OriginalMusic/originalmusic-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Original Music</h3>
                  <span>Music</span>
                </div>
              </div>
            </li>

            <li class="Patents grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Awards & Accolades"
                  data-category="Patents"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 8"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/Patents/patents-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Patents</h3>
                  <span>Patents</span>
                </div>
              </div>
            </li>

            <li class="Presentations grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Presentations"
                  data-category="Presentations"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 9"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/Presentations/presentations-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Presentations</h3>
                  <span>Speaking</span>
                </div>
              </div>
            </li>

            <li class="Publications grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Awards & Accolades"
                  data-category="Publications"
                >
                  <a
                    class="portfolio_popup"
                    href="#"
                    @click.prevent="active = 10"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="img/portfolio/Publications/publications-logo.png"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Publications</h3>
                  <span>Publications</span>
                </div>
              </div>
            </li>




            <!-- <li class="youtube grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Alexa Skills"
                  data-category="Alexa"
                >
                  <a
                    class="popup-youtube"
                    href="#"
                    @click.prevent="() => onClick('youtube', '7e90gBu4pas')"
                  >
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/1.jpg"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Mockup Shape</h3>
                  <span>Youtube</span>
                </div>
              </div>
            </li>
            <li class="vimeo grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Ave Bottle"
                  data-category="Vimeo"
                >
                  <a
                    class="popup-vimeo"
                    href="#"
                    @click.prevent="() => onClick('vimeo', '337293658')"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/2.jpg"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Ave Bottle</h3>
                  <span>Vimeo</span>
                </div>
              </div>
            </li>
            <li class="soundcloud grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Magic Art"
                  data-category="Soundcloud"
                >
                  <a
                    class="soundcloude_link mfp-iframe audio"
                    href="#"
                    @click.prevent="() => onClick('soundcloud', '471954807')"
                  >
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/3.jpg"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Magic Art</h3>
                  <span>Soundcloud</span>
                </div>
              </div>
            </li>
            <li class="popup grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Scott Felix"
                  data-category="Popup"
                >
                  <a
                    class="zoom"
                    href="#"
                    @click.prevent="() => onClick('img', 'img/portfolio/5.jpg')"
                  >
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/5.jpg"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Blue Lemon</h3>
                  <span>Popup</span>
                </div>
              </div>
            </li>
            <li class="popup grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  data-title="Art Stone"
                  data-category="Popup"
                >
                  <a
                    class="zoom"
                    href="#"
                    @click.prevent="() => onClick('img', 'img/portfolio/4.jpg')"
                  >
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/4.jpg"></div>
                  </a>
                </div>
                <div class="mobile_title">
                  <h3>Art Stone</h3>
                  <span>Popup</span>
                </div>
              </div>
            </li> -->
            
          </ul>
        </div>
      </div>
      <div class="brush_1 wow zoomIn" data-wow-duration="1s">
        <img src="/img/brushes/portfolio/1.png" alt="" />
      </div>
      <div class="brush_2 wow fadeInRight" data-wow-duration="1s">
        <img src="/img/brushes/portfolio/2.png" alt="" />
      </div>
    </div>
  </div>
  <MagnificPopUpVue
    :modal="modal"
    :close="closeModal"
    :name="name"
    :src="src"
  />
  <!-- ALEXA SKILLS -->
  <div :class="`${active === 2 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/Alexa/alexa-logo.png"
            style="background-image: url('img/portfolio/Alexa/alexa-logo.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Alexa Skills</h3>
          <span><a href="#">Alexa</a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="textbox" style="background-image: linear-gradient(to bottom right, white, grey)">
            <p>
              I write Alexa skills (applications) for Wabi Sabi Software. My most successful skill is Premier League which has been rated a "high engagement" skill by AWS
            </p>
            <p>
              <a 
                href="https://alexa-skills.amazon.com/apis/custom/skills/amzn1.ask.skill.ac0e64f9-bb6e-4c67-afb4-d4ff3a959f1f/launch"
                target="_blank"
                rel="noopener noreferrer"
              >
              Try Premier League
              </a>
            </p>
            <p>
              If you have a comment, question or suggestion please email us at BrianTarbox@gmail.com
            </p>
            <p>
              If you enjoy Premier League please consider giving us a review. If you did not like the skill please email and we will try to fix it. It's all about the beautiful game.
            </p>
            <p>
              If you are using an Alexa without a screen you can ask about the following things:
            </p>
            <p>
              <span style="font-weight: 800">
              table, results, fixtures, touches, tackles, fouls, clean sheets, goals, yellow cards, red cards, referees
              </span>
            </p>
            <p>
              If you are using an Alexa with a screen you can press any of these buttons:
            </p>
          </div>
          <div class="detailbox">
            <ul>
              <li>
                <span class="first">Client</span>
                <span>Wabi Sabi Software & others</span>
              </li>
              <li>
                <span class="first">Category</span>
                <span><a href="#">Alexa skills</a></span>
              </li>
              <li>
                <span class="first">Date</span>
                <span>2020-2023+</span>
              </li>
            </ul>
          </div>
        </div>
        <div class="additional_images">
          <ul>

            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/Alexa/alexa-1.png"
                    style="background-image: url('img/portfolio/Alexa/alexa-1.png')"
                  ></div>
                </div>
                <br/>
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/Alexa/alexa-2.png"
                    style="background-image: url('img/portfolio/Alexa/alexa-2.png')"
                  ></div>
                </div>
                <br/>
                <p>
                  If you select <span style="font-weight: 800">teams</span> you can get the form, fixtures or results for that team
                </p>
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/Alexa/alexa-3.png"
                    style="background-image: url('img/portfolio/Alexa/alexa-3.png')"
                  ></div>
                </div>
                <br/>
                <p>
                  <span style="font-weight: 800">
                    Alexa How To Videos
                  </span>
                </p>
                <p>
                  I've published a guide to using the Alexa APLA Audio Mixing directives.
                </p>
                <p>
                  <a 
                    href="https://www.youtube.com/watch?v=S9wwtKERFB8"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Tutorial Video
                  </a>
                </p>

                <p>
                  <a 
                    href="https://briantarbox.org/alexa_apla.zip"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Source Code for APLA Examples
                  </a>
                </p>

                <p>
                  I've also published a guide to using the Alexa APL Video directives.
                </p>

                <p>
                  <a 
                    href="https://youtu.be/5zqUdIQC3AM"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Tutorial Video
                  </a>
                </p>
                <p>
                  <a 
                    href="https://briantarbox.org/apl.zip"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Source Code for APL (Video) Examples
                  </a>
                </p>

              </div>
            </li>

            <!-- <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/Alexa/alexa-2.png"
                    style="background-image: url('img/portfolio/Alexa/alexa-2.png')"
                  ></div>
                </div>
              </div>
              
            </li> -->

            <!-- <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/2.jpg"
                    style="background-image: url('img/portfolio/2.jpg')"
                  ></div>
                </div>
              </div>
            </li> -->

            <!-- <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/3.jpg"
                    style="background-image: url('img/portfolio/3.jpg')"
                  ></div>
                </div>
              </div>
            </li> -->
          </ul>
        </div>
      </div>
    </ModalBox>
  </div>

  <!-- AWARDS -->
  <div :class="`${active === 3 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details" width="100%" padding-right="0px" margin-right="0px">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/Awards/awards-logo.png"
            style="background-image: url('img/portfolio/Awards/awards-logo.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Awards</h3>
          <span><a href="#">Awards</a></span>
          <div></div>
        </div>
        <div class="main_details" width="100%" padding-right="0px" margin-right="0px">
          <div class="portfolio_main_title">
            <p>
              Over the years I've won a few awards for my work, including Most Innovative use of Java,
              JavaOne Speaker Award, Most Innovative Use of Jira, NetWorld Product Of The Year, etc.
            </p><p>
              
              <img src="https://briantarbox.org/DukesChoice.jpg" height="200" width="200"/>
              <img src="https://briantarbox.org/RockStar.gif" height="200" width="200"/>
              <img src="https://briantarbox.org/CharlieAwards.png" height="200" width="200"/>
              <img src="https://briantarbox.org/IMG_8390.png" height="200" width="200"/>
              <img src="https://briantarbox.org/IMG_8391.png" height="200" width="200"/>
              <img src="https://briantarbox.org/pankration.jpg" height="200" width="200"/>
              <img src="https://briantarbox.org/million_streams.jpg" height="200" width="200"/>
            </p>
            <!-- <p>
              <a 
                href="https://alexa-skills.amazon.com/apis/custom/skills/amzn1.ask.skill.ac0e64f9-bb6e-4c67-afb4-d4ff3a959f1f/launch"
                target="_blank"
                rel="noopener noreferrer"
              >
              Try Premier League
              </a>
            </p>
            <p>
              If you have a comment, question or suggestion please email us at BrianTarbox@gmail.com
            </p>
            <p>
              If you enjoy Premier League please consider giving us a review. If you did not like the skill please email and we will try to fix it. It's all about the beautiful game.
            </p>
            <p>
              If you are using an Alexa without a screen you can ask about the following things:
            </p>
            <p>
              <span style="font-weight: 800">
              table, results, fixtures, touches, tackles, fouls, clean sheets, goals, yellow cards, red cards, referees
              </span>
            </p>
            <p>
              If you are using an Alexa with a screen you can press any of these buttons:
            </p>
          </div>
          <div class="detailbox">
            <ul>
              <li>
                <span class="first">Client</span>
                <span>Wabi Sabi Software & others</span>
              </li>
              <li>
                <span class="first">Category</span>
                <span><a href="#">Alexa skills</a></span>
              </li>
              <li>
                <span class="first">Date</span>
                <span>2020-2023+</span>
              </li>
            </ul>
          </div>
        </div>
        <div class="additional_images">
          <ul>

            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/Alexa/alexa-1.png"
                    style="background-image: url('img/portfolio/Alexa/alexa-1.png')"
                  ></div>
                </div>
                <br/>
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/Alexa/alexa-2.png"
                    style="background-image: url('img/portfolio/Alexa/alexa-2.png')"
                  ></div>
                </div>
                <br/>
                <p>
                  If you select <span style="font-weight: 800">teams</span> you can get the form, fixtures or results for that team
                </p>
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/Alexa/alexa-3.png"
                    style="background-image: url('img/portfolio/Alexa/alexa-3.png')"
                  ></div>
                </div>
                <br/>
                <p>
                  <span style="font-weight: 800">
                    Alexa How To Videos
                  </span>
                </p>
                <p>
                  I've published a guide to using the Alexa APLA Audio Mixing directives.
                </p>
                <p>
                  <a 
                    href="https://www.youtube.com/watch?v=S9wwtKERFB8"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Tutorial Video
                  </a>
                </p>

                <p>
                  <a 
                    href="https://briantarbox.org/alexa_apla.zip"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Source Code for APLA Examples
                  </a>
                </p>

                <p>
                  I've also published a guide to using the Alexa APL Video directives.
                </p>

                <p>
                  <a 
                    href="https://youtu.be/5zqUdIQC3AM"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Tutorial Video
                  </a>
                </p>
                <p>
                  <a 
                    href="https://briantarbox.org/apl.zip"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  Source Code for APL (Video) Examples
                  </a>
                </p> -->

              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>



  <!-- BAWSton -->
  <div :class="`${active === 4 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/BAWSton/bawston-logo.png"
            style="background-image: url('img/portfolio/BAWSton/bawston-logo.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>bAWSton User Group</h3>
          <span><a href="#">bAWSton, MA</a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="portfolio_main_title" style="background-image: linear-gradient(to bottom right, white, grey)">
            <p>
              The bAWSton User Group is one of the largest and longest running AWS UG's in the world.  
              During covid we met every other week ... trying to fill the void as most UGs suspended operations.<br>
              We have a well earned reputation for diversity, including having 58% of our 2021 speakers being women or POC.<br>
            Our meetings are still virtual as we've developed a following that either doesn't live in the Boston area or lives
            outside the US.<br>
            We are happy to provide a platform for Heros, Community Builders, cloud experts and cloud novices to all come together to learn.<br><br>

            </p>
                  <a 
                    href="https://www.meetup.com/the-boston-amazon-web-services-meetup-group/"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  The meetup page
                  </a> <br><br>
                 
                  <a 
                    href="https://studio.youtube.com/channel/UCbTkDEqqKxOiZ5F84JPuA_Q/videos/upload?filter=%5B%5D&sort=%7B%22columnType%22%3A%22date%22%2C%22sortOrder%22%3A%22DESCENDING%22%7D"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                  The meetup videos
                  </a>                      
              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>



  <!-- Certifications -->
  <div :class="`${active === 11 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/certifications.png"
            style="background-image: url('img/certifications.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Certifications</h3>
          <span><a href="#">Certifications</a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="portfolio_main_title" style="background-image: linear-gradient(to bottom right, white, grey)">
            <p>
              I have a number of certifications.  Most are technology related but I'm also a Rescue Diver and an Instrument Rated Private Pilot<br><br>
                <img src="img/certifications/aws-certified-alexa-skill-builder-specialty.png" height="300" width="385">
                <img src="img/certifications/aws-certified-database-specialty.png" height="300" width="385"><br>
                <img src="img/certifications/aws-certified-developer-associate.png" height="300" width="385">
                <img src="img/certifications/aws-certified-security-specialty.png" height="300" width="385"><br>
                <img src="img/certifications/aws-certified-solutions-architect-associate.png" height="300" width="385">
                <img src="img/certifications/terraform.png" height="300" width="385">
                <img src="img/certifications/Sumo.png" height="300" width="385">
                <img src="img/certifications/Splunk.png" height="300" width="385">
                <img src="img/certifications/privatepilot.jpg" height="300" width="385">
                <img src="img/certifications/PADI_rescue_diver.png" height="300" width="385">
             </p>                   
              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>


  <!-- Music -->
  <div :class="`${active === 7 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/OriginalMusic/Flutes.jpg"
            style="background-image: url('img/portfolio/OriginalMusic/Flutes.jpg')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Original Music</h3>
          <span><a href="#"></a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="textbox">
            <p>
              I play a variety of native style flutes, here is some of my music
            </p>
        <br/><br/><a href="didjeridoo1.mp3"> Didgeridoo </a>
        <br/><br/><a href="stellasMarch.mp3"> Stella's Wedding March </a> -->
        <br/><br/><a href="http://soundcloud.com/brian-tarbox"> Collection of songs on SoundCloud.com </a>
<br/><br/> Drone Flute  <audio controls>  <source src="drone2WithEcho.mp3" type="audio/mpeg">  Your browser does not support the audio tag.</audio>
<br/><br/> Stella March  <audio controls>  <source src="stellasMarch.mp3" type="audio/mpeg">  Your browser does not support the audio tag.</audio>
<br/><br/> Didjeridoo    <audio controls>  <source src="didjeridoo1.mp3" type="audio/mpeg">  Your browser does not support the audio tag.</audio>                  
              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>




  <!-- Dolphins -->
  <div :class="`${active === 5 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/Dolphins/dolphins-logo.png"
            style="background-image: url('img/portfolio/Dolphins/dolphins-logo.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Dolphins</h3>
          <span><a href="#"></a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="portfolio_main_title" style="background-image: linear-gradient(to bottom right, white, aqua)">
            <p>
              I worked at the Kewalo Basin Marine Mammal Laboratory (KBMML) doing language research with bottlenosed dolphins for the University of Hawaii.
My Master's thesis was a Prolog model of what we thought the dolphins thought about various experiments.
What we mostly discovered was that we humans were not as flexible in our thinking as we believed and that aquatic
creatures see (and hear) the world very differently than we do.
<br><br>
As an example, there was a Play Choice experiment where we offered two toys to the dolphins, they picked one and we gave it to them.<br><br>
They would then destroy the toy.  We were shocked and puzzled.   After literally months we once accidentally gave the dolphin the toy they
had not selected ... and they loved it.   In a binary choice they were telling us the item they did <strong>not</strong> want.  Completely 
arbitrary and appropriate and much too complex for the humans.<br><br>
            </p>
            <a href="https://web.archive.org/web/20150810075406/http://www.dolphin-institute.org/our_research/dolphin_research/abstracts/1988tarbox.html"><br/>Master Thesis Summary </a><br>
                <img src="img/dolphins/dolphin.jpg" height="300" width="385">
                <img src="img/dolphins/dolphins0.jpg" height="300" width="375">
                <img src="img/dolphins/dolphin1.jpg" height="300" width="375">
                <img src="img/dolphins/dolphin2.jpg" height="300" width="375">
                <img src="img/dolphins/dolphin3.jpg" height="300" width="375">
                <img src="img/dolphins/dolphin4.jpg" height="300" width="375">
                <img src="img/dolphins/ake.png" height="300" width="375">
                   
              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>



  <!-- Patents -->
  <div :class="`${active === 8 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/Patents/patents-logo.png"
            style="background-image: url('img/portfolio/Patents/patents-logo.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Granted Patents</h3>
          <span><a href="#"></a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="portfolio_main_title" style="background-image: linear-gradient(to bottom right, white, grey)">
            <p>
              I've been granted ten US Patents; Several patents were deemed broad enough to split into two separate patents
            </p>

         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=3&f=G&l=50&co1=AND&d=PTXT&s1=tarbox&s2=adaptive&OS=tarbox+AND+adaptive&RS=tarbox+AND+adaptive"> 10,476,923 Filtering Content for Adaptive Streaming </a>
        <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=2&f=G&l=50&co1=AND&d=PTXT&s1=tarbox.INNM.&s2=brian.INNM.&OS=IN/tarbox+AND+IN/brian&RS=IN/tarbox+AND+IN/brian"> 10,129,570 System and method for stream fault tolerance through usage based duplication and shadow sessions </a>
         <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=3&f=G&l=50&co1=AND&d=PTXT&s1=tarbox.INNM.&s2=brian.INNM.&OS=IN/tarbox+AND+IN/brian&RS=IN/tarbox+AND+IN/brian"> 9,998,775 Enforcement of trick-play disablement in adaptive bit rate video content delivery </a>
        <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=4&f=G&l=50&co1=AND&d=PTXT&s1=tarbox.INNM.&s2=brian.INNM.&OS=IN/tarbox+AND+IN/brian&RS=IN/tarbox+AND+IN/brian"> 9,537,920 Enforcement of trick-play disablement in adaptive bit rate video content delivery </a>
          <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=5&f=G&l=50&co1=AND&d=PTXT&s1=tarbox.INNM.&s2=brian.INNM.&OS=IN/tarbox+AND+IN/brian&RS=IN/tarbox+AND+IN/brian"> 9,497,489 System and method for stream fault tolerance through usage based duplication and shadow sessions </a>
          <br>
         <a href="http://appft1.uspto.gov/netacgi/nph-Parser?Sect1=PTO1&Sect2=HITOFF&d=PG01&p=1&u=/netahtml/PTO/srchnum.html&r=1&f=G&l=50&s1=20140297745.PGNR.&OS=DN/20140297745&RS=DN/20140297745"> 9,191,422 Processing of social media for selected time-shifted multimedia content </a>
          <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=1&f=G&l=50&co1=AND&d=PTXT&s1=tarbox&s2=CACHING&OS=tarbox+AND+CACHING&RS=tarbox+AND+CACHING"> 8,510,785 Adaptive media caching for video on demand  </a>
          <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=1&f=G&l=50&co1=AND&d=PTXT&s1=tarbox&s2=snover&OS=tarbox+AND+snover&RS=tarbox+AND+snover"> 6,664,987 System for displaying a computer managed network layout with transient display of user selected attributes of displayed network objects </a>
          <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=2&f=G&l=50&co1=AND&d=PTXT&s1=tarbox&s2=snover&OS=tarbox+AND+snover&RS=tarbox+AND+snover"> 6,101,498 System for displaying a computer managed network layout with a first transient display of a user selected primary attribute of an object and a supplementary transient display of secondary attributes  </a>
          <br>
         <a href="http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO2&Sect2=HITOFF&p=1&u=%2Fnetahtml%2FPTO%2Fsearch-bool.html&r=3&f=G&l=50&co1=AND&d=PTXT&s1=tarbox&s2=snover&OS=tarbox+AND+snover&RS=tarbox+AND+snover"> 6,020,889 System for displaying a computer managed network layout with varying transience display of user selected attributes of a plurality of displayed network objects </a>
                   
              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>



  <!-- Presentations -->
  <div :class="`${active === 9 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/Presentations/presentations-logo.png"
            style="background-image: url('img/portfolio/Presentations/presentations-logo.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Presentations</h3>
          <span><a href="#"></a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="portfolio_main_title" style="background-image: linear-gradient(to bottom right, white, grey)">

        <img src="img/presentations/logicast_4_10.png" height="250" width="355"/><br>
        <a href="https://www.youtube.com/watch?v=JwMKZH2G5uY">Logicast AWS New Roundup</a><br><br>


        <img src="img/presentations/Werner_keynote_2025.png" height="250" width="355"/><br>
        <a href="https://www.linkedin.com/feed/update/urn:li:activity:7270552970616856577/">Werner Vogels 2025 re:Invent Keynote</a><br><br>

        <img src="img/presentations/cloudzero.png" height="250" width="355"/><br>I was part of the CloudZero / Anthropic / Caylent Lightning talk at re:Invent<br><br>

        <img src="img/presentations/Garman_keynote_2025.png" height="250" width="355"/><br>
        <a href="https://www.linkedin.com/feed/update/urn:li:activity:7269814346912800768/">Matt Garman 2025 re:Invent Keynote</a><br><br>

        <img src="img/presentations/Silly.png" height="250" width="355"/><br>
        <a href="https://www.tiktok.com/@caylent/video/7406404346918866206?fbclid=IwY2xjawFam6dleHRuA2FlbQIxMAABHYEwLzlNC9nUs_VwfPgdU-wf-WITHMSzV_IySTydH1mtPdaEkCYR7uc3QQ_aem_kHH77ro0sQOkJZPVzgDG0Q">Caylent did a silly video of me at re:Invent</a><br><br>

        <img src="img/presentations/Logicata.png" height="250" width="355"/><br>
        <a href="https://logicastvideo.podbean.com/e/season-3-episode-16-certifications-snowmobiles-and-large-language-models/">Logicata: Certifications, Snowmobiles, and Large Language Models</a><br><br>

        <img src="img/presentations/Ukraine.png" height="250" width="355"/><br>
        <a href="https://www.youtube.com/watch?v=kY_M3bbojO4">DevOpsDay (Ukraine):Let's Talk Security (go to 2:15:38)</a><br><br>

        <img src="img/presentations/NeuralNebulAI_10.png" height="250" width="325"/><br>
        <a href="https://www.youtube.com/watch?v=PcGuAQrmGh8">Caylent Neural NebulAI Episode 10: Leveraging Data Inside of AI</a><br><br>

        <img src="img/presentations/NeuralNebulAI_8.png" height="250" width="325"/><br>
        <a href="https://www.youtube.com/watch?v=0zEWG19XRIc">Caylent Neural NebulAI Episode 8: Pre-AI Data Monderization & Enablement</a><br><br>

        <img src="img/presentations/NeuralNebulAI_5.png" height="250" width="325"/><br>
        <a href="https://www.youtube.com/watch?v=d6XPYeyRBrs">Caylent Neural NebulAI Episode 5: Foundation Models</a><br><br>

        <img src="img/presentations/CheckingOutCodeWhisperer.png" height="250" width="325"/><br>
        <a href="https://www.youtube.com/watch?v=0jxOoGsKPls">Checking out Amazon Code Whisperer</a><br><br>

        <img src="img/presentations/NeuralNebulAI_4.png" height="250" width="325"/><br>
        <a href="https://www.linkedin.com/events/humans-ai-neuralnebulaiepisode47114645196386013184/comments/">Caylent Neural NebulAI Episode 4: Humans and AI</a><br><br>

        <img src="img/presentations/NeuralNebulAI_2.png" height="250" width="325"/><br>
        <a href="https://www.youtube.com/watch?v=3zcth3OwYfs">Caylent Neural NebulAI Episode 2: Unwrapping AI and GenAI</a><br><br>

        <img src="img/presentations/NeuralNebulAI_1.png" height="250" width="275"/><br>
        <a href="https://www.youtube.com/watch?v=iDyrhOmJkXQ">Caylent Neural NebulAI Episode 1: Ethics</a><br><br>

        <a href="https://www.youtube.com/watch?v=4LEi7DZ5ydk">New Voices - advice from a hero</a><br><br>

        <img src="img/presentations/AWS_Developers_podcast.jpg" height="250" width="275"/><br>
        <a href="https://open.spotify.com/episode/2kgGsOXGlYsOFISTNV8iqd">AWS Developers Podcast with Dave Isbitsky and Emily Freeman. Episode 089 - Thoughts on Serverless</a><br><br>

        <img src="img/presentations/logicast.png" height="250" width="475"/><br>
        <a href="https://logicast.podbean.com/e/season-2-episode-23-cloud-costs-cloud-heroes-cloud-villains/">Cloud Costs, Cloud Heroes, Cloud Villains</a><br><br>

        <img src="img/presentations/DeveloperInnovationDays.png" height="250" width="475"/><br>
        <a href="https://briantarbox.org/Tarbox_at_DevInovationDay.mp4">Cameo appearance to talk about CodeWhisperer</a><br><br>

        <img src="img/presentations/AWS_Developers_podcast.jpg" height="250" width="275"/><br>
        <a href="https://podcasts.apple.com/us/podcast/aws-developers-podcast/id1574162669">AWS Developers Podcast with Dave Isbitsky and Emily Freeman. Episode 059 - CodeWhisperer</a><br><br>
        Voice22: Emotions and Customer Satisfaction<br>
        <i>
Top Alexa skill builder Brian Tarbox's presentation outlined how skills that evoke an emotional response are more engaging to the user and tend to generate higher satisfaction. Brian knows that emotions are key to brand recognition and loyalty. He's also aware that providing these kinds of experiences might be easier said than done, so he also walked us through the code required to make this happen. His talk can teach you to leverage new Alexa emotions and speaking styles to create naturally engaging voice experiences.
        </i><br>
        <div class="row">
          <div class="column">
            <img src="img/presentations/BrianAtVoice22.png" height="250"/>
          </div>
          <div class="column">
            <img src="img/presentations/Brian2AtVoice22.png" height="250"/>
          </div>
        </div>
        
        <br><br><br>
 
        <img src="img/presentations/AlexaOfficeHours.png" height="250" width="475"/><br>
        <a href="https://www.youtube.com/watch?v=xq7rkMLSQJ0">Office Hours featuring expert Alexa developer, Brian Tarbox</a><br><br>
        <img src="img/presentations/vBrownBag.png" height="250" width="475"/><br>
        <a href="https://vbrownbag.com/2022/03/episode-followup-add-in-skill-purchasing-to-your-alexa-skill-presented-by-brian-tarbox/">Add In-Skill Purchasing to your Alexa Skill</a><br><br>


        VBrownBag Interview
        <a href="https://www.youtube.com/watch?v=fo_QwlSQL-E&t=17s">Interview with Chris Williams</a><br><br><br>
        Developer's Lounge: Verner Vogals Keynote Instant Reaction Panel<br>
        <img src="img/presentations/instantreaction.jpg" height="250" width="275"/>
        <img src="img/presentations/heros.jpg" height="250" width="275"/>
        <img src="img/presentations/verner_selfi.jpg" height="250" width="275"/> <br>
        User Group Leader Meeting: How to grow your MeetUp and Its Diversity<br>
        <img src="img/presentations/UG_talk.jpg" height="250" width="275"/>
        <img src="img/presentations/IMG_7870_skip.jpg" height="250" width="275"/> <br>

         <br>NY ML AWS MeetUp, September, 2022 <i>CodeWhisperer</i> <a href="Amazon+CodeWhisperer+by+Brian+Tarbox2.mp4">Presentation Video</a><br>
        <br>Denver AWS MeetUp, April, 2021 <i>Building Your First Alexa Skill</i> <a href="https://www.youtube.com/watch?v=pS0oyrOT-iAa">Presentation Video</a><br>
        <br>IndyAWS MeetUp, March, 2021 <i>Making An Alexa Skill Feel More Natural</i> <a href="https://youtu.be/4LyQy-Aq79o">Presentation Video</a><br>
        <br>Charlotte AWS MeetUp, February, 2021 <i>Community Panel</i> <a href="https://www.youtube.com/watch?v=d7G7_jvta30&feature=youtu.be">Presentation Video</a><br>
        <br>Boston AWS MeetUp, January, 2021 <i>re:Invent 2020  TLDR</i> <a href="https://youtu.be/Cn7vHHWOkDQ">Presentation Video</a><br>
        <br>Boston AWS MeetUp, October, 2020 <i>Comparing CloudFormation and Terraform</i> <a href="https://youtu.be/b6WUA8vSslM?t=322">Presentation Video</a>
        <br/>
        <br>Dublin AWS Meetup, February 14, 2020 <i>Machine Learning and Serverless</i> <br/><img height="360" width="480" src="img/presentations/Dublin_aws_meetup.jpg"><br/>
        <br/>
        <br>Boston AWS Meetup, March 28, 2019 <i>Lambda Deep Dive</i> <a href="https://vimeo.com/327300612/a55cea1693">Presentation Video</a>
        <br/>
        <br/>Boston Alexa Meetup, November, 2017 <i>PremierLeague, an Alexa skill</i>
        <br/><img height="360" width="480" src="img/presentations/AlexaTalk.jpg"><br/>

        <br/>
        <br/>Boston AWS Meetup, September, 2017 <i>PremierLeague, an Alexa skill</i>
        <br/>
        <br/>AWS Portsmouth User Group, April, 2017 <i>AWS Overview and Introduction to Alexa</i>
        <br/>
        <br/>Boston AWS Meetup, August, 2016, "<i>More Screen Time, An Alexa Skill</i>"
        <br/>
        <br/>MetroWest Coders, January, 2016 "<i>AWS Overview</i>" <a href="https://www.youtube.com/watch?v=mDktLJ95ZhM">Presentation Video</a>
        <br/>
        <br/>New England Java User's Group, January, 2016 "<i>AWS Overview With Selected Deep Dives</i>"
        <br/>
        <br/>New England Java User's Group, October, 20http://localhost:8080/img/presentations/coolbeans.gif15 "<i>Running Cassandra in the Cloud</i>"
        <br/>
        <br/>Boston AWS Meetup, March 2014 <i>Using Spot Instances in Use Cases One Might Not Have Thought About</i>"
        <br/>
        <br/>Boston AWS Meetup, July, 2013 <i>AWS Infrastructure Automation Tools, Scripts, and Tips</i> (one of several speakers giving informal talks)
        <br/>
        <br/>New England Java Users Group: March 2012, <i>Scala Open Source Case Study</i>
        <br/>
        <br/><a href="https://www.slideshare.net/briantarbox/2012-ncta-motorolaintelligent-caching-and-packaging-in-an-abr-multiformat-cdn-tarboxfinal">Presentation Slides</a>
        <br/>NCTA Spring Technical Forum, Boston, May 2012, “Intelligent Caching in an ABR Multi-Format CDN World” 
        <br/>
        <br/>JavaOne 2012, “Advanced Beginner Scala” 
        <br/><br/>
JavaOne 2009, Programming Music for Fun and Productivity; a talk about converting any program’s log file into a music string so as to debug your program like an auto mechanic listens to your car. 
        <br/>
        <br/> <a href="https://bplskillimages.s3.amazonaws.com/Moto_Summit.mp4">Making The Switch</a>
        <br/>Atlassian Summit 2010 ,“Making the Switch”, a presentation on innovative ways to use Eclipse, Mylyn and Jira as both an integrated development system and a training library. Received Charlie Award for Innovation.
        <br/>

        <br/><a href="https://ieeexplore.ieee.org/abstract/document/196141">Talk Abstract</a>
        <br/>"User Modeling at a dolphin language laboratory", presented to the IEEE 1988 conference on Artificial Intelligence Applications, San Diego, CA. 
        <br/>
        <br/>Led the Boston Architectural Kata Practitioners October meeting on designing an ROV system
        <br/>
        <br/>"Easel: A User Interface Management Tool", presented at 1985 ACM SIGCHI. 

              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>



  <!-- Publications -->
  <div :class="`${active === 10 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/Publications/publications-logo.png"
            style="background-image: url('img/portfolio/Publications/publications-logo.png')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Publications</h3>
          <span><a href="#"></a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="portfolio_main_title" style="background-image: linear-gradient(to bottom right, white, grey)">
            <p>
              Over the years I've been published in a variety of places
            </p>
            <a href="https://caylent.com/blog/getting-started-with-agentic-ai-on-aws">January 2025, <em>Getting Started with Agentic AI on AWS</em></a>
            <br><br>
            <a href="https://caylent.com/blog/scaling-ml-to-meet-customer-demand-and-reduce-errors">October 2024, <em>Scaling ML to Meet Customer Demand and Reduce Errors</em></a>
            <br><br>
            <a href="https://caylent.com/blog/optimizing-aws-data-pipelines-for-compliance-in-digital-advertising">April 2024, <em>Optimizing AWS Data Pipelines for Compliance in Digital Advertising</em></a>
            <br><br>
            <a href="https://dev.to/btarbox/why-resilience-matters-21d4">March 2024, <em>Why Resilience Matters</em></a>
            <br><br>
            <a href="https://dev.to/aws-heroes/certification-is-not-enough-98j">March 2024, <em>Certification is not enough</em></a>
            <br><br>
            <a href="https://dev.to/btarbox/certification-tips-from-an-aws-hero-n16">March 2024, <em>Certification Tips from an AWS Hero</em></a>
            <br><br>
            <a href="https://dev.to/btarbox/running-an-inclusive-and-engaging-aws-user-group-i0i">March 2024, <em>Running ann Inclusive and Engaging AWS User Group</em></a>
            <br><br>
            <a href="https://dev.to/btarbox/enhancing-data-security-with-s3-object-lock-1je4">March 2024, <em>Enhancing Data Security with S3 Object Lock</em></a>
            <br><br>
            <a href="https://caylent.com/blog/swami-sivasubramanian-keynote-recap-aws-re-invent-2023">December 2023, <em>Swami Sivasubramanian Keynote Recap</em></a>
            <br><br>
            <a href="https://caylent.com/blog/werner-vogels-keynote-recap-aws-re-invent-2023">December 2023, <em>Werner Vogels Keynote Recap</em></a>
            <br><br>
            <a href="https://dev.to/btarbox/the-future-of-alexa-skills-211j">October 2023, <em>The Future Of Alexa Skills</em></a>
            <br><br>
            I was quoted in a Financials Times article about Amazon Alexa
            <a href="https://enterprise-sharing.ft.com/redeem/5e67e3b4-2db9-4086-b973-aafc24fe6a45">February 2023, <em>Amazon's big dreams for Alexa fall short</em></a>

            <br><br>An article AWS wrote about me
            <a href="https://developer.amazon.com/en-US/blogs/alexa/alexa-skills-kit/2022/05/Alexa-skill-insights-brian-tarbox-premier-league-may-20221">May 2022,
            <em>The Alexa Skills Insights Team helped the skill PremierLeague boost discovery and increase users</em></a>
            <br><br>

            <a href="https://dev.to/btarbox/finally-understanding-outposts-and-local-zones-5d91">September 2023, Dev.to 
            <em>Finally Understanding Outposts and Local Zones</em></a>
            <br><br>
            <a href="https://dev.to/aws-heroes/exploring-the-options-for-billing-and-capacity-reservations-53o3">June 2023, Dev.to 
            <em>Exploring The Options For Billing And Capacity Reservations</em></a>
            <br><br>
            <a href="https://dev.to/aws-heroes/a-confusion-that-costs-3808">October 2023, Dev.to 
            <em>A Confusion That Costs</em></a>
            <br><br>
            <a href="https://dev.to/aws-heroes/time-to-rethink-cattle-vs-pets-serverless-5c0j">October 2023, Dev.to 
            <em>Time to rethink cattle vs pets</em></a>
            <br><br>

            <h3>Sym.io</h3>
            <a href="https://blog.symops.com/2023/01/27/aws-performance-testing//">January 2023,
            <em>Save Time and Money On AWS By Running Performance Tests</em></a>
            <br><br>
            <a href="https://blog.symops.com/2022/08/31/amazon-codewhisperer/">August 2022,
            <em>Can Amazon's CodeWhisperer Write Better Python Than You?</em></a>
            <br><br>
            <a href="https://blog.symops.com/2022/08/17/lambda-guardrails/">August 2022,
            <em>Three Guardrails For AWS Lambda</em></a>
            <br><br>
            <a href="https://blog.symops.com/2022/08/10/pay-for-continuous-integration/">August 2022,
            <em>Should You Pay For CI/CD In 2020?</em></a>
            <br><br>
            <a href="https://blog.symops.com/2022/07/07/prevent-ransomware-s3-object-lock/">July 2022,
            <em>Protect Your Data From Ransomware with S3 Object Lock</em></a>
            <br><br>

            <h3>SearchAWS.com</h3>
            <a href="http://searchaws.techtarget.com/feature/Serverless-AI-lead-reInvent-2017-expert-predictions">November 2017,
            <em>re:Invent Predictions"</em></a><br>
            <a href="http://searchaws.techtarget.com/tip/Five-Alexa-tricks-to-build-better-more-interactive-skills"><br />October 2017, <em>Five Alexa tricks to build better, more interactive skills</em></a><br>
            <a href="http://searchaws.techtarget.com/tip/Dive-into-AWS-Lambda-example-code-for-S3-alerts"><br />January 2016, <em>Dive into AWS Lambda example code for S3 alerts</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/Set-up-and-configure-an-AWS-Lambda-function"><br />January 2016, <em>Set up and configure an AWS Lambda function</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/AWS-Config-add-on-automates-AWS-tags-creation"><br />June 2015, <em>AWS Config add-on automates AWS tags creation</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/AWS-nudging-users-toward-HVM-instance-type"><br />June 2015, <em>AWS nudging users toward HVM instance type</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/Wrangle-AWS-Spot-Instances-with-Spot-Fleets-and-save"><br />June 2015, <em>Wrangle AWS Spot Instances with Spot Fleets and save</em></a><br />
            <a href="http://searchaws.techtarget.com/opinion/Docker-on-AWS-Its-not-you-its-me"><br />April 2015, <em>Its not you Docker, its me</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/Cost-of-running-Docker-containers-vs-AWS-instances"><br />May 2014, <em>Cost of running Docker Containers vs. AWS Instances</em></a><br />
            <a href="http://tinyurl.com/p6wdmj5"><br />May 2014, <em>Demystifying AWS and Docker</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/Spoiler-alert-Your-AWS-application-isnt-that-mission-critical"><br />May 2014, <em>Your Mission's Not That Critical</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/Combat-a-common-error-with-AWS-EC2-instances"><br />May 2014, <em>Combatting a common error with AWS EC2 Instances</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/The-inner-workings-of-AWS-AutoScaling"><br />May 2014, <em>The Inner Workings of AWS AutoScaling</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/Set-up-AWS-CloudWatch-alerts-and-alarms"><br />May 2014, <em>Setup AWS CloudWatch Alerts and Alarms</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/AWS-CloudWatch-terms-and-definitions"><br />April 2014, <em>AWS CloudWatch Terms and Definitions</em></a><br />
            <a href="http://searchaws.techtarget.com/tip/Setting-up-your-first-AWS-account"><br />March 2014, <em>Setting up your first AWS account</em></a><br /><br />

          <h3>LinkedIn Articles</h3>
          <a href="https://www.linkedin.com/in/briantarbox/detail/recent-activity/posts/"><br /> <em>My LinkedIn Pulse News Articles</em></a><br /><br />

          <h3>National Cable Television Annual Meeting</h3>
          <a href="papers/Complexity_Considerations_NCTA.pdf"> Complexity Considerations for Centralized vs Remote Packaging.  NCTA May 2012</a><br/><br>
          <a href="papers/IntelligentCaching_NCTA.pdf"> Intelligent Caching In An ABR Multi-formation CND World.  NCTA May 2012</a><br/>

          <br/>
          <h3>No Fluff, Just Stuff</h3>
          April 2012, <em>Scala Case Study: Rewriting an Open Source Music Program (part 2</em>), No Fluff, Just Stuff<br/><br>
          March 2012, <em>Scala Case Study: Rewriting an Open Source Music Program (part 1))</em>, No Fluff, Just Stuff<br/><br>
          December 2011, <em>Knowns and Unknowns of Agile</em>, No Fluff, Just Stuff<br/>

          <h3>Pragmatic Programmer Magazine</h3>
          <a href="https://www.dropbox.com/s/4qwy26krq4cykuv/AppsVsWebFinal.pdf"><br />October 2013, <em>Apps vs. Web</em></a><br />
          <a href="http://pragprog.com/magazines/2012-12/agile-in-the-small"><br />December 2012, <em>Agile in the Small</em></a><br />
          <a href="http://pragprog.com/magazines/2012-06/retrospective-velocity"><br />March 2012, <em>Retrospective Velocity</em></a><br />
          <a href="http://pragprog.com/magazines/2012-03/comparing-java-and-scalas-expressiveness"><br />March 2012, <em>Comparing Scala and Java's Expressiveness</em></a><br />
          <a href="http://pragprog.com/magazines/2011-<br />12/justintime-logging"><br />December 2011, <em>A new approach to logging</em></a><br />
          <a href="http://pragprog.com/magazines/2011-11/root-cause-analysis-from-long-ago" rel="nofollow"><br />November 2011, <em>The long history of root cause analysis</em></a><br /><br />
          <a href="http://pragprog.com/magazines/2011-09/scala-traits">Sept 2011 <em>Scala Traits For The Java Programmer</em></a><br /><br />
          <a href="http://pragprog.com/magazines/2011-08/code-as-dialog">August 2011 <em>Code As Dialog</em> </a><br/><br>
          <a href="http://pragprog.com/magazines/2011-05/catch-the-pig">May 2011                           <em>Catch the Pig!                 </em></a><br/><br>
          <a href="http://rubylearning.com/blog/2010/10/25/the-value-of-a-personal-bug-log">November 2010 <em>The value of a personal bug log</em></a><br/><br>
          <a href="http://pragprog.com/magazines/2010-09/the-key-to-better-software">September 2010        <em>The Key to Better Software</em> </a><br/><br />
          <a href="http://pragprog.com/magazines/2010-06/better-tools-and-training">June 2010       <em>Better Tools and Training</em> </a><br /><br/>
          <a href="http://pragprog.com/magazines/2010-05/the-floating-finish-line">May 2010         <em>The Floating Finish Line</em> </a><br /><br />
          <a href="http://pragprog.com/magazines/2010-04/medicine-making-music">April 2010          <em>Medicine Making Music</em> </a><br /><br />
          <a href="http://pragprog.com/magazines/2010-03/testing-as-contract">March 2010            <em>Testing As Contract</em> </a><br /><br />
          <a href="http://pragprog.com/magazines/2009-11/interrupt-mood">November 2009              <em>Interrupt Mood</em> </a><br /><br /><br>
          <a href="http://pragprog.com/magazines/2009-09/and-your-bugs-can-sing">June 2009          <em>...And Your Bugs Can Sing</em> </a>
          <br/><br/>


          <h3>Dr Dobbs</h3>
          <a href="http://drdobbs.com/database/218100564">June 2010 <em>Debugging MySQL Stored Procedures</em> </a><br /><br />

          <h3>Seven Languages in Seven Weeks by Bruce Tate</h3>
          <a href="http://media.pragprog.com/titles/btlang/prolog.pdf">June 2010 <em>Interviewed as Prolog SME</em> </a><br /><br />

          <h3>IEEE</h3>
          <a href="http://https://ieeexplore.ieee.org/document/196141/authors#authors">March 1988 <em>User Modeling at a Dolphin Language Laboratory</em> </a><br /><br />

<br/>
I am also one of the co-authors of the New England Java Group's 2002 book: <em>"Coding Standards for Java"</em>

              </div>
            <!-- </li> -->
          <!-- </ul> -->
        </div>
      </div>
    </ModalBox>
  </div>



</template>

<script>
import MagnificPopUpVue from "./popup/MagnificPopUp.vue";
import ModalBox from "./popup/ModalBox.vue";
export default {
  name: "PortfolioComponent",
  data() {
    return {
      activeNav: "1", // props
      name: "",
      src: "",
      modal: false,
      // Content
      active: 0,
    };
  },
  mounted() {
    let Isotope = require("isotope-layout");
    setTimeout(() => {
      let iso = new Isotope(".gallery_zoom", {
        itemSelector: ".grid-item",
        //    layoutMode: "fitRows",
        percentPosition: true,
        masonry: {
          columnWidth: ".grid-item",
        },
        animationOptions: {
          duration: 750,
          easing: "linear",
          queue: false,
        },
      });
      let filterFns = {
        // show if number is greater than 50
        numberGreaterThan50: function (itemElem) {
          let number = itemElem.querySelector(".number").textContent;
          return parseInt(number, 10) > 50;
        },
        // show if name ends with -ium
        ium: function (itemElem) {
          let name = itemElem.querySelector(".name").textContent;
          return name.match(/ium$/);
        },
      };
      // bind filter button click filter main funtion
      let filtersElem = document.querySelector(".portfolio_filter ul");
      filtersElem.addEventListener("click", function (event) {
        if (event.target.getAttribute("data-filter")) {
          let filterValue = event.target.getAttribute("data-filter");
          filterValue = filterFns[filterValue] || filterValue;
          iso.arrange({ filter: filterValue });
        }
      });
    }, 1000);
  },
  methods: {
    onClick(name, src) {
      this.name = name;
      this.src = src;
      this.modal = true;
    },
    closeModal() {
      this.modal = false;
      this.name = "";
      this.src = "";
    },
    close() {
      this.active = 0;
    },
  },
  components: { MagnificPopUpVue, ModalBox },
};
</script>

<template>
  <div class="dizme_tm_section">
    <div class="dizme_tm_copyright">
      <div class="container">
        <div class="inner">
          <div class="left wow fadeInLeft" data-wow-duration="1s">
            
            <p>
              Copyright &copy; 2008-{{ new Date().getFullYear() }}
              <a href="http://briantarbox.blogspot.com/" target="_blank" rel="noopener noreferrer">
                Brian Tarbox
              </a>
              (<a href="mailto:briantarbox@gmail.com" style="text-decoration: underline; font-weight: 300;">briantarbox@gmail.com</a>).
              All rights reserved.
            </p>
           
            <p>
              Developed with ♥ + 💻 by
              <a href="https://brianhhough.com" target="_blank" rel="noopener noreferrer">
                Brian H. Hough
              </a
              >
              
            </p>
          </div>
          <div class="right wow fadeInRight" data-wow-duration="1s">
            <ul>
              <li><a href="#">Terms &amp; Condition</a></li>
              <li><a href="#">Privacy Policy</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CopyrightComponent",
  components: {},
};
</script>

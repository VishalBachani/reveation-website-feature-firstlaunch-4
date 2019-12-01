<template>
  <footer class="rl-footer">
    <div class="rl-footer-top">
        <b-container>
            <b-row>

          <b-col lg="3" md="6" class="footer-info">
            <h3>Reveation Labs </h3>
            <p></p>
          </b-col>

          <b-col lg="3" md="6" class="footer-links">
            <h4>Useful Links</h4>
            <ul>
              <li><font-awesome-icon :icon="['fas', 'angle-right']"></font-awesome-icon><a href="#">Home</a></li>
              <li><font-awesome-icon :icon="['fas', 'angle-right']"></font-awesome-icon><a href="#">About us</a></li>
              <li><font-awesome-icon :icon="['fas', 'angle-right']"></font-awesome-icon><a href="#">Services</a></li>
              <li><font-awesome-icon :icon="['fas', 'angle-right']"></font-awesome-icon><a href="#">Terms of service</a></li>
              <li><font-awesome-icon :icon="['fas', 'angle-right']"></font-awesome-icon><a href="#">Privacy policy</a></li>
            </ul>
          </b-col>

          <b-col lg="3" md="6" class="footer-contact">
            <h4>Contact Us</h4>
            <p>
              A108 Adam Street <br>
              New York, NY 535022<br>
              United States <br>
              <strong>Phone:</strong> +1 5589 55488 55<br>
              <strong>Email:</strong> info@example.com<br>
            </p>

            <div class="social-links">
              <a href="#" class="linkedin"><font-awesome-icon :icon="['fab', 'linkedin']"></font-awesome-icon></a>
              <a href="#" class="twitter"><font-awesome-icon :icon="['fab', 'twitter']"></font-awesome-icon></a>
              <a href="#" class="facebook"><font-awesome-icon :icon="['fab', 'facebook']"></font-awesome-icon></a>
              <a href="#" class="instagram"><font-awesome-icon :icon="['fab', 'instagram']"></font-awesome-icon></a>
            </div>

          </b-col>

          <b-col lg="3" md="6" class="footer-newsletter">
            <h4>Our Newsletter</h4>
            
            <form action="" method="post">
              <input type="email" name="email"><input type="submit"  value="Subscribe">
            </form>
          </b-col>

        </b-row>    
        </b-container>
    </div>

    <div class="container">
      <div class="copyright">
        &copy; Copyright <strong>BizPage</strong>. All Rights Reserved
      </div>
      <div class="credits">
        <!--
          All the links in the footer should remain intact.
          You can delete the links only if you purchased the pro version.
          Licensing information: https://bootstrapmade.com/license/
          Purchase the pro version with working PHP/AJAX contact form: https://bootstrapmade.com/buy/?theme=BizPage
        -->
        Designed by <a href="https://bootstrapmade.com/">BootstrapMade</a>
      </div>
    </div>
  </footer><!-- .rl-footer -->
</template>

<script>
export default {
  data() {
    return {
      message: "Try change me!"
    };
  },
  methods: {
    onClick() {
      this.message = "Here you go :)";
    }
  }
};
</script>

<style>
.rl-footer {
    background: #000;
    padding: 0 0 30px;
    color: #eee;
    font-size: 14px;
}
.rl-footer .rl-footer-top {
    background: #111;
    padding: 60px 0 30px;
}

.rl-footer .rl-footer-top .footer-info {
  margin-bottom: 30px;
}

.rl-footer .rl-footer-top .footer-info h3 {
  font-size: 34px;
  margin: 0 0 20px 0;
  padding: 2px 0 2px 10px;
  line-height: 1;
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  letter-spacing: 3px;
  border-left: 4px solid #18d26e;
}

.rl-footer .rl-footer-top .footer-info p {
  font-size: 14px;
  line-height: 24px;
  margin-bottom: 0;
  font-family: "Montserrat", sans-serif;
  color: #eee;
}

.rl-footer .rl-footer-top .social-links a {
  font-size: 18px;
  display: inline-block;
  background: #333;
  color: #eee;
  line-height: 1;
  padding: 8px 0;
  margin-right: 4px;
  border-radius: 50%;
  text-align: center;
  width: 36px;
  height: 36px;
  transition: 0.3s;
}

.rl-footer .rl-footer-top .social-links a:hover {
  background: #18d26e;
  color: #fff;
}

.rl-footer .rl-footer-top h4 {
  font-size: 14px;
  font-weight: bold;
  color: #fff;
  text-transform: uppercase;
  position: relative;
  padding-bottom: 12px;
}

.rl-footer .rl-footer-top h4::before,
.rl-footer .rl-footer-top h4::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: 0;
  height: 2px;
}

.rl-footer .rl-footer-top h4::before {
  right: 0;
  background: #555;
}

.rl-footer .rl-footer-top h4::after {
  background: #18d26e;
  width: 60px;
}

.rl-footer .rl-footer-top .footer-links {
  margin-bottom: 30px;
}

.rl-footer .rl-footer-top .footer-links ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.rl-footer .rl-footer-top .footer-links ul a {
  padding-left: 8px;  
}

.rl-footer .rl-footer-top .footer-links ul li {
  border-bottom: 1px solid #333;
  padding: 10px 0;
}

.rl-footer .rl-footer-top .footer-links ul li:first-child {
  padding-top: 0;
}

.rl-footer .rl-footer-top .footer-links ul a {
  color: #eee;
}

.rl-footer .rl-footer-top .footer-links ul a:hover {
  color: #18d26e;
  text-decoration: none;
}

.rl-footer .rl-footer-top .footer-contact {
  margin-bottom: 30px;
}

.rl-footer .rl-footer-top .footer-contact p {
  line-height: 26px;
}

.rl-footer .rl-footer-top .footer-newsletter {
  margin-bottom: 30px;
}

.rl-footer .rl-footer-top .footer-newsletter input[type="email"] {
  border: 0;
  padding: 6px 8px;
  width: 65%;
}

.rl-footer .rl-footer-top .footer-newsletter input[type="submit"] {
  background: #18d26e;
  border: 0;
  width: 35%;
  padding: 6px 0;
  text-align: center;
  color: #fff;
  transition: 0.3s;
  cursor: pointer;
}

.rl-footer .rl-footer-top .footer-newsletter input[type="submit"]:hover {
  background: #13a456;
}

.rl-footer .copyright {
  text-align: center;
  padding-top: 30px;
}

.rl-footer .credits {
  text-align: center;
  font-size: 13px;
  color: #ddd;
}
</style>
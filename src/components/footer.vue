<template>
  <div>
    <div class="footer-content">
      <div class="first-footer-container">
        <logo :footer="footer" />
        <div class="social-icon-container">
          <facebook-icon />
          <youtube-icon />
          <twitter-icon />
          <pinterest-icon />
          <instagram-icon />
        </div>
      </div>
      <div class="second-footer-container">
        <p>About Us</p>
        <p>Contact</p>
        <p>Blog</p>
      </div>
      <div class="third-footer-container">
        <p>Careers</p>
        <p>Support</p>
        <p>Privacy Policy</p>
      </div>
      <div class="fourth-footer-container">
        <button class="button">Request Invite</button>
        <h5>&copy; Easybank. All Rights Reserved</h5>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from "../images/logo";
import FacebookIcon from "../images/facebook-icon";
import YoutubeIcon from "../images/youtube-icon";
import TwitterIcon from "../images/twitter-icon";
import PinterestIcon from "../images/pinterest-icon";
import InstagramIcon from "../images/instagram-icon";

export default {
  components: {
    Logo,
    FacebookIcon,
    YoutubeIcon,
    TwitterIcon,
    PinterestIcon,
    InstagramIcon
  },
  data() {
    return {
      footer: true
    };
  }
};
</script>
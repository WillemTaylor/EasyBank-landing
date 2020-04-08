<template>
  <div>
    <logo :header="header" style="margin-top: 14px;" />
    <div class="shortcuts mobile-hide">
      <p>Home</p>
      <p>About</p>
      <p>Contact</p>
      <p>Blog</p>
      <p>Careers</p>
    </div>
    <hamburger-icon class="hamburger desktop-hide" />
    <button class="button mobile-hide">Request Invite</button>
  </div>
</template>

<script>
import Logo from "../images/logo";
import HamburgerIcon from "../images/hamburger-icon";

export default {
  components: {
    Logo,
    HamburgerIcon
  },
  data() {
    return {
      header: true
    };
  }
};
</script>
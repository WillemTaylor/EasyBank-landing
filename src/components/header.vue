<template>
  <div class="header-container">
    <logo :header="header" />
    <hamburger-icon class="hamburger" />
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
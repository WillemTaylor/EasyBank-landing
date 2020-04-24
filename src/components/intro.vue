<template>
  <div>
    <div class="image-container">
      <div v-if="isMobile" class="bg-mobile">
        <intro-bg-mob />
      </div>
      <div v-else class="bg-desktop">
        <intro-bg-desktop />
      </div>
      <img class="image-phones" :src="image" />
    </div>
    <div class="intro-container">
      <h1>Next generation digital banking</h1>
      <p>Take your financial life online. Your Easybank account will be a one-stop shop for spending, saving, budgeting, investing and much more.</p>
      <button class="button">Request Invite</button>
    </div>
  </div>
</template>

<script>
import IntroBgMob from "../images/intro-bg-mob";
import IntroBgDesktop from "../images/intro-bg-desktop";
import image from "../images/image-phones.png";

export default {
  components: {
    IntroBgMob,
    IntroBgDesktop
  },
  data() {
    return {
      image: image,
      screenWidth: window.innerWidth
    };
  },
  computed: {
    isMobile() {
      return this.screenWidth < 960;
    }
  },
  mounted() {
    window.addEventListener("resize", () => {
      this.screenWidth = window.innerWidth;
    });
  }
};
</script>
<template>
  <div>
    <div class="image-container">
      <!-- Had to use 'v-if screenWidth' here rather than a 'display: block / hide' media query, as the whole desktop image wouldn't show when setting display: none; on the mobile image for some reason. You can imitate by adding 'desktop-hide' and 'mobile-hide' classes to 'bg-mobile' and 'bg-desktop' respectively -->
      <div v-if="screenWidth < 1200" class="bg-mobile">
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
      screenWidth: screen.width
    };
  }
};
</script>
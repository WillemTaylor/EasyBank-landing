<template>
  <div>
    <div class="image-container">
      <intro-bg-mob class="bg-mobile" />
      <img class="image-mockups" :src="image" />
    </div>
    <h1>Next generation digital banking</h1>
    <p>Take your financial life online. Your Easybank account will be a one-stop shop for spending, saving, budgeting, investing and much more.</p>
    <button class="button">Request Invite</button>
  </div>
</template>

<script>
import IntroBgMob from "../images/intro-bg-mob";
import image from "../images/image-mockups.png";

export default {
  components: {
    IntroBgMob
  },
  data() {
    return {
      image: image
    };
  }
};
</script>
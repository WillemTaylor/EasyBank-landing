<template>
  <div>
    <h1>Latest Articles</h1>
    <div class="articles-container">
      <div class="article-container">
        <img :src="currency" />
        <h6>By Claire Robinson</h6>
        <h4>Receive money in any currency with no fees</h4>
        <p>The world is getting smaller and we're becoming more mobile.So why should you be forced to only receive money in a single...</p>
      </div>

      <div class="article-container">
        <img :src="restaurant" />
        <h6>By Wilson Hutton</h6>
        <h4>Treat yourself without worrying about money</h4>
        <p>Our simple budgeting feature allows you to separate out your spending and set realistic limits each month. That means you...</p>
      </div>

      <div class="article-container">
        <img :src="plane" />
        <h6>By Wilson Hutton</h6>
        <h4>Take your Easybank card wherever you go</h4>
        <p>We want you to enjoy your travels.This is why we don't charge any fees on purchases while you're abroad. We'll even show...</p>
      </div>

      <div class="article-container">
        <img :src="confetti" />
        <h6>By Claire Robinson</h6>
        <h4>Our invite-only Beta accounts are now live!</h4>
        <p>After a lot of hard work by the whole team, we're excited to launch our closed beta. It's easy to request an invite through the site...</p>
      </div>
    </div>
  </div>
</template>

<script>
import currency from "../images/image-currency.jpg";
import restaurant from "../images/image-restaurant.jpg";
import plane from "../images/image-plane.jpg";
import confetti from "../images/image-confetti.jpg";

export default {
  data() {
    return {
      currency: currency,
      restaurant: restaurant,
      plane: plane,
      confetti: confetti
    };
  }
};
</script>
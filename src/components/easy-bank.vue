<template>
  <div>
    <Header />
    <Intro class="intro" />
    <why-choose class="why-choose" />
    <latest-articles class="latest-articles" />
    <Footer class="footer" />
  </div>
</template>

<script>
import Header from "./header";
import Intro from "./intro";
import WhyChoose from "./why-choose";
import LatestArticles from "./latest-articles";
import Footer from "./footer";

export default {
  name: "EasyBank",
  components: {
    Header,
    Intro,
    WhyChoose,
    LatestArticles,
    Footer
  }
};
</script>

<template>
  <div>
    <logo :header="header" />
    <nav role="navigation">
      <div id="menuToggle">
        <input type="checkbox" />
        <span></span>
        <span></span>
        <span></span>
        <ul id="menu">
          <a href="#">
            <li>Home</li>
          </a>
          <a href="#about">
            <li>About</li>
          </a>
          <a href="#contact">
            <li>Contact</li>
          </a>
          <a href="#blog">
            <li>Blog</li>
          </a>
          <a href="#careers">
            <li>Careers</li>
          </a>
        </ul>
      </div>
    </nav>
    <button class="button mobile-hide">Request Invite</button>
  </div>
</template>

<script>
import Logo from "../images/logo";

export default {
  components: {
    Logo
  },
  data() {
    return {
      header: true
    };
  }
};
</script>
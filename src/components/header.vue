<template>
  <div>
    <logo :header="header" />
    <div class="shortcuts mobile-hide">
      <p>Home</p>
      <p>About</p>
      <p>Contact</p>
      <p>Blog</p>
      <p>Careers</p>
    </div>
    <div class="desktop-hide">
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
            <a href="#">
              <li>About</li>
            </a>
            <a href="#">
              <li>Contact</li>
            </a>
            <a href="#">
              <li>Blog</li>
            </a>
            <a href="#">
              <li>Careers</li>
            </a>
          </ul>
        </div>
      </nav>
    </div>
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
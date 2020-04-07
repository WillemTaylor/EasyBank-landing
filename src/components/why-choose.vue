<template>
  <div>
    <h1>Why choose Easybank?</h1>
    <p>We leverage Open Banking to turn your bank account into your financial hub. Control your finances like never before.</p>
    <online-banking class="online-banking" />
    <h3>Online Banking</h3>
    <p>Our modern web and mobile applications allow you to keep of your finances wherever you are in the world.</p>
    <Budgeting />
    <h3>Simple Budgeting</h3>
    <p>See exactly where your money goes each month. Receive notifications when you're close to hitting your limits.</p>
    <Onboarding />
    <h3>Fast Onboarding</h3>
    <p>We don't do branches. Open your account in minutes online and start taking control of your finances right away.</p>
    <Api />
    <h3>Open API</h3>
    <p>Manage your savings, investments, pension and much more from one account. Tracking your money has never been easier.</p>
  </div>
</template>

<script>
import OnlineBanking from "../images/online-banking";
import Budgeting from "../images/budgeting";
import Onboarding from "../images/onboarding";
import Api from "../images/api";

export default {
  components: {
    OnlineBanking,
    Budgeting,
    Onboarding,
    Api
  }
};
</script>
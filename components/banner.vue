<template>
  <div class="bg-black">
    <div class="bg-banner">
      <div class="banner">
        <h2>
          <span>we're</span> the edmonton framing contractor
        </h2>
        <p>any projects large or small</p>
        <p>edmonton and around</p>
      </div>
      <div class="banner-btn text-lg">
          <a :href="telLink">
            <img src="../assets/images/icons8-phone-50.png" alt=""/>
          </a>
          <a :href="telLink">Call us at 1-780-271-6505</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    telLink() {
      const phoneNumber = "17802716505"; // Remplacez par votre numéro de téléphone
      return `tel:${phoneNumber}`;
    },
  },
};
</script>

<style lang="css">

.bg-banner {
  height: 83vh;
}
.bg-banner::before {
  content: "";
  background-image: url("../assets/images/homeImg.jpg");
}

</style>

<template>
  <div class="bg-black">
    <div class="bg-banner">
      <div class="banner">
        <div>
          <h2>
            <span>we are </span><br>the edmonton framing contractor
          </h2>
        </div>
        <p>any projects <span>large or small</span></p>
        <p>edmonton and <span>around</span></p>
        <button class="banner-btn text-lg mt-16">

          <a :href="telLink">
            <img src="../assets/images/icons8-phone-50.png" alt=""/>
          </a>
          <a :href="telLink">Call us at 1-780-271-6505</a>
        </button>
      </div>
      <!-- <div class="banner-btn text-lg"> -->
      <!-- </div> -->
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
  background-image: url("../assets/images/logo_official.svg"), url("../assets/images/homeImg.jpg") ;
  background-position: center, center; /* Positionnement au centre pour les deux images */
  background-size: contain, cover; /* Ajustement de la taille pour les deux images */
  background-repeat: no-repeat;
}

</style>

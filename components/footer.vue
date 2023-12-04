<template>
    <div class="footer-container">
      <div class="footer-sub-container">
        <div class="footer-contact-info">
          <h3>
            <span>East Claw Construction Inc.</span>
          </h3>
          <p>
            <a
              :href="googleMapsLink"
              >Edmonton, Alberta</a
            >
          </p>
          <p>
            <a class="hover:text-[#e42b00] ease-in duration-200" :href="telLink"
              >1-780-271-6505</a
            >
          </p>
          <p>
            <a
              href="mailto:EastClawConstructionInc@hotmail.com"
            >
              eastclawconstructioninc@hotmail.com
            </a>
          </p>
        </div>
        <div class="footer-about-us">
          <h3>
            <span>About Us</span>
          </h3>
          <p>
            East Claw Construction Inc. is an experienced carpenter in the
            Edmonton area specializing in the construction and repair of
            residential and commercial buildings. Our experts offer you
            professional service, superior quality products and competitive
            prices! East Claw construction inc is the reference for structural
            work.
          </p>
        </div>
      </div>
      <div class="footer-copyright">
        <p>
          Copyright 2022 © LA TOILE TECHNOLOGIE
        </p>
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
    googleMapsLink() {
      const address = " Edmonton, Alberta"; // Remplacez par l'adresse de votre entreprise
      const encodedAddress = encodeURIComponent(address);
      return `https://www.google.com/maps/search/?api=1&query=${encodedAddress}`;
    },
  },
};
</script>

<style scoped>


</style>

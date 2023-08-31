<template>
  <div class="footer-div bg-black">
    <div class="footer-container mx-auto px-4 py-8 footer-container">
      <div class="sm:flex">
        <div
          class="flex flex-col w-full sm:w-1/2 mb-14 justify-start items-center"
        >
          <h3 class="info-footer mb-4">
            <span>East Claw Construction Inc.</span>
          </h3>
          <p class="text-[#fff] mb-4">
            <a
              class="hover:text-[#e42b00] ease-in duration-200"
              :href="googleMapsLink"
              >9151 Shaw Way, Edmonton, Alberta</a
            >
          </p>
          <p class="text-[#fff] mb-4">
            <a class="hover:text-[#e42b00] ease-in duration-200" :href="telLink"
              >1-780-271-6505</a
            >
          </p>
          <p class="text-[#fff]">
            <a
              class="hover:text-[#e42b00] ease-in duration-200"
              href="mailto:EastClawConstructionInc@hotmail.com"
            >
              eastclawconstructioninc@hotmail.com
            </a>
          </p>
        </div>
        <div class="flex flex-col items-center w-full sm:w-1/3">
          <h3 class="info-footer mb-4">
            <span>About Us</span>
          </h3>
          <p class="text-[#fff]">
            East Claw Construction Inc. is an experienced carpenter in the
            Edmonton area specializing in the construction and repair of
            residential and commercial buildings. Our experts offer you
            professional service, superior quality products and competitive
            prices! East Claw construction inc is the reference for structural
            work.
          </p>
        </div>
      </div>
      <div class="flex flex-col text-center sm:text-left">
        <p id="info-hv" class="mt-8 text-gray-400 text-xs text-center">
          Copyright 2022 © LA TOILE TECHNOLOGIE
        </p>
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
    googleMapsLink() {
      const address = "9151 Shaw Way, Edmonton, Alberta"; // Remplacez par l'adresse de votre entreprise
      const encodedAddress = encodeURIComponent(address);
      return `https://www.google.com/maps/search/?api=1&query=${encodedAddress}`;
    },
  },
};
</script>

<style scoped>
.footer-div {
  padding: 0 0 50px 0;
  border-top: 3px solid #e4002b;
}

.footer-container {
  margin-top: 50px;
}

.info-footer {
  color: #e4002b;
}

#info-hv {
  margin-top: 15px;
  color: #ededed;
  font-size: 12px;
}
</style>

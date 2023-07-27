<template>
  <div>
    <div
      class="bg-frey border-4 border-black bg-center bg-fixed overflow-hidden flex justify-center items-center align-center"
    >
      <div
        class="flex flex-col items-start text-justify justify-center align-center w-5/6 md:w-4/6 lg:w-3/6"
      >
        <h2
          class="text-[#e42b00] text-center justify-center items-center text-4xl md:text-5xl lg:text-6xl font-bold relative mb-8 md:mb-12"
        >
          <span class="text-[#fff]">Contact&nbsp;</span> Us
        </h2>
        <p
          class="text-[#fff] font-bold text-base md:text-xl relative mb-6 md:mb-10 pb-2"
        >
          Take advantage of our hassle-free, no-obligation estimates! Just send
          us an email with your name, address, contact number and details of
          your project including any photos, drawings or plans. We'll be in
          touch within 24 hours.
        </p>
        <NuxtLink
          to="/contact"
          class="btn text-white bg-transparent relative font-bold border-2 border-white lg:py-4 md:py-3 sm:py-3 py-3 px-6 md:px-8 hover:text-[#e42b00] ease-in duration-200"
          >Contact Us Now
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<style>
.bg-frey {
  margin-top: 0;
  padding-right: 0rem !important;
  position: relative;
  height: 60vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #171717 !important;
  overflow-x: hidden;
}

.bg-frey::before {
  background-attachment: fixed;
  content: "";
  background-image: url("../assets/images/frey-cropped.jpg");
  background-position: top center;
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  opacity: 0.7;
}

@media (max-width: 768px) {
  .bg-frey {
    height: 70vh;
  }

  .bg-frey::before {
    background-position: center center;
  }
}
</style>

<template>
  <div class="h-3/6">
    <div
      class="bg-frey bg-center bg-fixed -max overflow-hidden flex justify-center items-center align-center"
    >
      <div
        class="flex flex-col items-start text-justify justify-center align-center w-3/6"
      >
        <h2
          class="text-[#e42b00] text-center justify-center items-center text-6xl font-bold relative mb-4"
        >
          <span class="text-[#fff]">Contact&nbsp;</span> Us
        </h2>
        <p class="text-[#fff] font-bold text-xl relative mb-10 pb-2">
          Take advantage of our hassle-free, no-obligation estimates! Just send
          us an email with your name, address, contact number and details of
          your project including any photos, drawings or plans. We'll be in
          touch within 24 hours.
        </p>
        <NuxtLink
          to="/contact"
          class="btn text-white bg-transparent relative font-bold border-2 border-white py-4 px-6 hover:text-[#e42b00]"
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
  /* padding: 260px 0 100px 0 !important; */
  position: relative;
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #171717 !important;
  overflow-x: hidden;
}
.bg-frey::before {
  content: "";
  background-image: url("../assets/images/frey-cropped.jpg");
  background-position: top center;
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
  opacity: 70%;
}
</style>

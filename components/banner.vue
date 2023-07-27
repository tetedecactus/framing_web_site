<template>
  <div class="container bg-black">
    <div
      class="bg-homeImg pr-[-4] border-4 border-black bg-center bg-fixed h-screen overflow-hidden"
    >
      <div class="flex justify-start items-start">
        <div class="flex flex-col items-start text-justify mx-auto my-auto">
          <h2
            class="banner-title mt-10 flex text-white text-justify justify-start items-center text-2xl sm:text-2xl md:text-4xl lg:text-6xl font-bold relative mb-4"
          >
            <span class="text-[#e42b00]">WE'RE THE&nbsp;</span> EDMONTON FRAMING
          </h2>
          <h2
            class="flex text-white text-justify justify-center items-center text-xl sm:text-2xl md:text-4xl lg:text-6xl font-bold relative mb-16"
          >
            CONTRACTOR
          </h2>
          <p
            class="banner-p text-[#fff] font-bold text-md sm:text-sm md:text-lg lg:text-xl relative mb-10 pb-2"
          >
            ANY PROJECT LARGE OR SMALL
          </p>
          <p
            class="text-[#fff] font-bold text-md sm:text-sm md:text-lg lg:text-xl relative mb-10 pb-2"
          >
            EDMONTON AND AROUND
          </p>
          <div
            class="gradient-btn flex flex-row border-4 border-[#e42b00] relative text-lg py-4 px-6 rounded-none"
          >
            <a :href="telLink"
              ><img
                class="mr-4 relative hover:scale-[1.15] ease-in duration-300"
                src="../assets/images/icons8-phone-50.png"
                width="30"
                alt=""
            /></a>
            <a
              class="btn text-white bg-transparent relative font-bold hover:text-[#e42b00] ease-in duration-200"
              :href="telLink"
              >Call us at 1-780-271-6505</a
            >
          </div>
        </div>
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

<style>
.bg-homeImg {
  margin-top: 0;
  padding-right: 0rem !important;
  /* padding: 260px 0 100px 0 !important; */
  position: relative;
  height: 85vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #171717 !important;
  overflow-x: hidden;
}
.bg-homeImg::before {
  background-attachment: fixed;
  content: "";
  background-image: url("../assets/images/homeImg.jpg");
  background-position: top center;
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
  opacity: 40%;
}

@media (max-width: 1032px) {
  .bg-homeImg {
    height: 70vh;
  }

  .bg-frey::before {
    background-position: center center;
  }
  h2 {
    font-size: 55px !important;
  }
}

@media (max-width: 968px) {
  h2 {
    font-size: 42px !important;
  }
}

@media (max-width: 768px) {
  h2 {
    font-size: 35px !important;
  }
}

@media (max-width: 768px) {
  h2 {
    font-size: 35px !important;
  }
}
</style>

<template>
  <div class="container bg-black w-screen">
    <div
      class="bg-homeImg bg-center bg-fixed h-screen -max overflow-hidden flex justify-start items-start"
    >
      <div class="flex flex-col  items-start text-justify">
        <h2
          class="flex text-white text-justify justify-start items-center text-6xl font-bold relative mb-4"
        >
           <span class="text-[#e42b00]">WE'RE THE&nbsp;</span> EDMONTON FRAMING
        </h2>
        <h2
          class="flex text-white text-justify justify-center items-center text-6xl font-bold relative mb-16"
        >
          CONTRACTOR
        </h2>
        <p class="text-[#fff] font-bold text-xl relative mb-10 border-b-2 pb-2">
          ANY PROJECT LARGE OR SMALL
        </p>
        <p class="text-[#fff] font-bold text-xl relative mb-10 border-b-2 pb-2">
          EDMONTON AND AROUND
        </p>
        <div class="flex flex-row border-2 border-white text-lg py-4 px-6 rounded-none ">
          <img class="mr-4" src="../assets/images/icons8-phone-50.png" width="30" alt="">
          <NuxtLink
            to="/contact"
            class="btn text-white bg-transparent relative font-bold hover:text-[#e42b00]"
            >Call us at 1-780-271-6505
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.bg-homeImg {
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
.bg-homeImg::before {
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
</style>

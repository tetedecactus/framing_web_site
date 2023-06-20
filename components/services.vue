<template>
  <div
    class="bg-newConstruction mb-20 border-4 border-black bg-center bg-fixed h-screen -max overflow-hidden justify-center items-center flex flex-col"
  >
    <div class="flex-col flex justify-center align-center w-3/5">
      <h3
        class="mt-10 relative text-white text-6xl text-center ml-14 mb-10 font-bold"
      >
        <span class="text-[#e42b00]">Our&nbsp;</span> Services
      </h3>
      <p
        class="relative text-white text-4xl text-center text-justify ml-14 mb-10"
      >
        We provide services and products that set hight standards for quality,
        reliability, durability and value for money
      </p>
    </div>
    <div class="flex flex-row align-center justify-center mb-20">
      <div
        class="border-2 border-black relative service-one flex flex-col w-2/6 bg-white pb-4"
      >
        <img class="h-96" src="../assets/images/block.jpg" alt="" />
        <h3 class="text-2xl font-bold text-center h-10">
          Multi Family Residential Building
        </h3>
      </div>
      <div
        class="border-2 border-black relative service-two flex flex-col w-2/6 mx-8 bg-white"
      >
        <img class="h-96" src="../assets/images/home-half-done.jpg" alt="" />
        <h3 class="mt-4 text-2xl font-bold text-center h-10">
          Single Family Residential
        </h3>
      </div>
      <div
        class="border-2 border-black relative service-three flex flex-col w-2/6 bg-white pb-4"
      >
        <img class="h-96" src="../assets/images/garage_3.jpg" alt="" />
        <h3 class="mt-4 text-2xl font-bold text-center justify-center h-10">
          Accessory Building
        </h3>
      </div>
    </div>
  </div>
</template>

<style>
.bg-newConstruction {
  margin-top: 0;
  padding-right: 0rem !important;
  /* padding: 260px 0 100px 0 !important; */
  position: relative;
  height: 85vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgb(255, 255, 255);
  background: radial-gradient(
    circle,
    rgba(255, 255, 255, 1) 0%,
    rgba(0, 0, 0, 0.6727065826330532) 100%
  );
  overflow-x: hidden;
}
.bg-newConstruction::before {
  background-attachment: fixed;
  content: "";
  background-image: url("../assets/images/framing-of-a-new-house.jpg");
  background-position: top center;
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
  opacity: 60%;
}
</style>

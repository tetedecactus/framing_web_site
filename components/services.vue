<template>
  <div
    class="bg-services"
  >
    <div class="service-title-div">
      <h3>
        <span>Our&nbsp;</span> Services
      </h3>
      <p>
        We provide services and products that set hight standards for quality,
        reliability, durability and value for money
      </p>
    </div>
    <div class="service-img-div">
      <div
      >
        <img class="h-96 border-black border-b-2" src="../assets/images/block.jpg" alt="" />
        <h3 class="service-info">
          Multi Residential Building
        </h3>
      </div>
      <div
      >
        <img class="h-96 border-black border-b-2" src="../assets/images/home-half-done.jpg" alt="" />
        <h3 class="service-info">
          Single Family Residential
        </h3>
      </div>
      <div
      >
        <img class="h-96 border-black border-b-2" src="../assets/images/garage_3.jpg" alt="" />
        <h3 class="service-info">
          Accessory Building
        </h3>
      </div>
    </div>
  </div>
</template>

<style>
.bg-services {
  height: auto;
}
.bg-services::before {
  content: "";
  background-image: url("../assets/images/framing-of-a-new-house.jpg");
}
::-webkit-scrollbar {
    width: 0.1em;
    background-color: #000;
  }
  ::-webkit-scrollbar-thumb {
    background-color: #000000;

  }
</style>

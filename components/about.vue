<template>
  <div class="container h-auto w-screen bg-[#fff] mb-24">
    <div class="sub-container flex flex-col">
    <div class="flex flex-row align-center justify-center py-24">
      <div class="flex flex-col w-2/5 align-center justify-center">
        <h4 class="text-lg text-[#e42b00] font-bold ml-14 mb-14 font-bold">
          Trusted Professionals
        </h4>
        <h3 class="text-black text-6xl text-justify ml-14 mb-10 font-bold">
          Edmonton Framing<br />
          Construction
        </h3>
        <p
          class="text-black text-xl w-3/4 text-center text-justify ml-14 mb-10"
        >
          We specialize in commercial and residential wood framing structures in
          Edmonton, Alberta and surrounding areas. With years of experience, we
          deliver exceptional results tailored to your needs. Contact us today
          for a consultation!
        </p>
        <button
          to="/contact"
          class="w-1/3 btn text-white border-2 border-black text-lg py-4 ml-14 rounded-none bg-[#e42b00] hover:text-black"
        >
          Learn More
        </button>
      </div>
      <div class="w-2/5 flex flex-col justify-center relative">
        <img width="150" class="quality absolute" src="../assets/images/prenium-quality.png" alt="">
        <img
          class="flex border-4 border-black align-center justify-center"
          width="500"
          src="../assets/images/home-1.jpg"
          alt=""
        />
      </div>
    </div>
    </div>
  </div>
</template>


<style>
    .quality {
        top: -50px;
        right: 50%;
    }
</style>
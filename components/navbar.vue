<template>
  <section>
    <header class="bg-white">
      <nav
        class="container mx-auto mb-4 flex flex-col text-black h-24 items-center w-auto bg-white"
      >
        <div
          class="info flex flex-row bg-[#000] h-auto w-screen justify-between gap-10 px-32 text-white"
        >
          <p class="">1-780-271-6505</p>
          <p>
            <a href="mailto:EastClawConstructionInc@hotmail.com">
              eastclawconstructioninc@hotmail.com
            </a>
          </p>
        </div>
        <div class="flex flex-row">
          <NuxtLink to="/" class="flex lg:w-1/3 items-center justify-center">
            <img
              class="h-28 w-auto mx- hover:scale-1.05"
              src="../assets/images/letter_logo.svg"
              alt="Logo"
              width="200"
            />
          </NuxtLink>
          <div
            class="flex flex-row w-screen items-center justify-center bg-white"
          >
            <div class="lg:w-1/3 flex justify-center align-center">
              <ul class="flex gap-4 font-bold text-bold uppercase">
                <li>
                  <NuxtLink class="hover:border-b-2 hover:border-[#e42b00]" to="/about"
                    >About</NuxtLink
                  >
                </li>
                <li>
                  <NuxtLink class="hover:border-b-2 hover:border-[#e42b00]" to="/about"
                    >Our Projects</NuxtLink
                  >
                </li>
                <li>
                  <NuxtLink class="hover:border-b-2 hover:border-[#e42b00]" to="/about"
                    >Careers</NuxtLink
                  >
                </li>
              </ul>
            </div>
            <div class="flex align-center justify-center">
              <ul class="">
                <li>
                  <NuxtLink
                    to="/contact"
                    class="btn text-white border-2 border-black text-lg font-bold py-4 px-6 rounded-none bg-[#e42b00] hover:text-black"
                    >Contact Us
                  </NuxtLink>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </nav>
    </header>
  </section>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false, // Variable de données pour suivre l'état du menu
    };
  },
};
</script>

<style></style>

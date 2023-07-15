<template>
  <section>
    <header class="bg-white">
      <nav
        class="container mx-auto flex flex-col text-black h-32 items-center w-auto bg-white"
      >
        <div
          class="info flex flex-row bg-[#000] h-auto w-screen justify-between gap-10 px-32 text-white"
        >
        <div class="phone flex flex-row">
          <a :href="telLink"><img class="mr-2" src="../assets/images/icons8-phone-50.png" width='20' alt=" phone"></a>
          <p><a class="hover:text-[#e42b00] ease-in duration-200" :href="telLink">1-780-271-6505</a></p>

        </div>
        <div class="flex flex-row">
          <img class="mr-2" src="../assets/images/mail_icon.svg" width="20" alt="">
          <p>
            <a class="hover:text-[#e42b00] ease-in duration-200" href="mailto:EastClawConstructionInc@hotmail.com">
              eastclawconstructioninc@hotmail.com
            </a>
          </p>
        </div>
        </div>
        <div class="flex flex-row">
          <NuxtLink to="/" class="flex lg:w-1/3 items-center justify-center">
            <img
              class="logo h-32 w-full hover:scale-[1.15] ease-in duration-300"
              src="../assets/images/letter_logo.svg"
              alt="Logo"
              width="200"
            />
          </NuxtLink>
          <div
            class="flex flex-row w-screen items-center justify-center bg-white"
          >
            <div class="lg:w-2/3 flex justify-center align-center">
              <ul class="flex gap-4 font-bold text-bold uppercase text-md">
                <li class="space-x-4">
                  <NuxtLink
                    class="hover:border-b-2 hover:border-[#e42b00] ease-in duration-200"
                    to="/about"
                    >About</NuxtLink
                  >
                </li>
                <li>
                  <NuxtLink
                    class="hover:border-b-2 hover:border-[#e42b00] ease-in duration-200"
                    to="/service"
                    >Services</NuxtLink
                  >
                </li>
                <li>
                  <NuxtLink
                    class="hover:border-b-2 hover:border-[#e42b00] ease-in duration-200"
                    to="/project"
                    >Our Projects</NuxtLink
                  >
                </li>
                <li>
                  <NuxtLink
                    class="hover:border-b-2 hover:border-[#e42b00] ease-in duration-200"
                    to="/career"
                    >Careers</NuxtLink
                  >
                </li>
                <li>
                  <NuxtLink
                    class="hover:border-b-2 hover:border-[#e42b00] ease-in duration-200"
                    to="/contact"
                    >Contact Us</NuxtLink
                  >
                </li>
              </ul>
            </div>
            <div class="flex align-center justify-center">
              <ul class="m">
                <li>
                  <NuxtLink
                    to="/contact"
                    class="btn text-white border-2 border-black text-lg font-bold py-4 px-6 rounded-none bg-[#e42b00] hover:text-black ml-10 ease-in duration-200"
                    >Free Quote
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
      isOpen: false,
    };
  },
  computed: {
    telLink() {
      const phoneNumber = '17802716505'; // Remplacez par votre numéro de téléphone
      return `tel:${phoneNumber}`;
    },
  }
};
</script>

<style></style>

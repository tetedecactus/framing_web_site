<template>
  <nav class="navbar">
    <div
      class="nav-contact-info"
    >
      <div>
        <a :href="telLink"
          ><img
            src="../assets/images/icons8-phone-50.png"
            width="20"
            alt=" phone"
        /></a>
        <p>
          <a :href="telLink"
            >1-780-271-6505</a
          >
        </p>
      </div>
      <div>
        <img
          src="../assets/images/icons8-email-50.png"
          width="20"
          alt=""
        />
        <p>
          <a
            href="mailto:EastClawConstructionInc@hotmail.com"
          >
            eastclawconstructioninc@hotmail.com
          </a>
        </p>
      </div>
    </div>

    <div class="navbar-section">
      <!-- Header logo -->
      <NuxtLink to="/" class="logo">
        <img
          src="../assets/images/letter_logo.svg"
          alt="Logo"
          width="200"
        />
      </NuxtLink>

      <!-- Mobile toggle -->
      <div class="mobile-menu">
        <button @click="drawer">
          <svg
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path d="M4 6h16M4 12h16M4 18h16"></path>
          </svg>
        </button>
      </div>

      <!-- Navbar -->
      <div class="main-nav">
        <ul>
          <li>
            <NuxtLink
              class="custom-link"
              to="/about"
              >About</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              class="custom-link"
              to="/service"
              >Services</NuxtLink
            >
          </li>
          <!-- <li>
            <NuxtLink
            class="custom-link"
              to="/project"
              >Our Projects</NuxtLink
            >
          </li> -->
          <li>
            <NuxtLink
            class="custom-link"
              to="/career"
              >Careers</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
            class="custom-link"
              to="/contact"
              >Contact Us</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              to="/contact"
              class="nav-btn"
              >Free Quote</NuxtLink
            >
          </li>
        </ul>
      </div>

      <!-- Dark Background Transition -->
      <transition
        enter-class="opacity-0"
        enter-active-class="ease-out transition-medium"
        enter-to-class="opacity-100"
        leave-class="opacity-100"
        leave-active-class="ease-out transition-medium"
        leave-to-class="opacity-0"
      >
        <div
          @keydown.esc="isOpen = false"
          v-show="isOpen"
          class="z-10 fixed inset-0 transition-opacity"
        >
          <div
            @click="isOpen = false"
            class="absolute inset-0 bg-black opacity-50"
            tabindex="0"
          ></div>
        </div>
      </transition>

      <!-- Drawer Menu -->
      <aside
        class="mobile-nav p-5 transform top-0 left-0 w-64 bg-white fixed h-full overflow-auto ease-in-out transition-all duration-300 z-30"
        :class="isOpen ? 'translate-x-0' : '-translate-x-full'"
      >
        <div class="close">
          <button
            class="absolute top-0 right-0 mt-4 mr-4"
            @click="isOpen = false"
          >
            <svg
              class="w-6 h-6"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path d="M6 18L18 6M6 6l12 12"></path>
            </svg>
          </button>
        </div>

        <span
          @click="isOpen = false"
          class="flex w-full items-center p-4 border-b"
        >
          <Tailwind />
        </span>

        <ul class="font-sans">
          <li>
            <NuxtLink
              to="/about"
              @click="isOpen = false"
              class="custom-mobile-link"
              >About</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              to="/service"
              @click="isOpen = false"
              class="custom-mobile-link"
              >Services</NuxtLink
            >
          </li>
          <!-- <li>
            <NuxtLink
              to="/project"
              @click="isOpen = false"
              class="custom-mobile-link"
              >Our Projects</NuxtLink
            >
          </li> -->
          <li>
            <NuxtLink
              to="/career"
              @click="isOpen = false"
              class="custom-mobile-link"
              >Careers</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              to="/contact"
              @click="isOpen = false"
              class="custom-mobile-link"
              >Contact Us</NuxtLink
            >
          </li>
          <li class="pt-10">
            <NuxtLink
              to="/contact"
              @click="isOpen = false"
              class="mobile-btn"
              >Free Quote</NuxtLink
            >
          </li>
        </ul>
      </aside>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    drawer() {
      this.isOpen = !this.isOpen;
    },
  },
  watch: {
    isOpen: {
      immediate: true,
      handler(isOpen) {
        if (process.client) {
          if (isOpen) document.body.style.setProperty("overflow", "hidden");
          else document.body.style.removeProperty("overflow");
        }
      },
    },
  },
  mounted() {
    document.addEventListener("keydown", (e) => {
      if (e.keyCode == 27 && this.isOpen) this.isOpen = false;
    });
  },
  computed: {
    telLink() {
      const phoneNumber = "17802716505";
      return `tel:${phoneNumber}`;
    },
  },
};
</script>

<style>
@media screen and (max-width: 880px) {
  .main-nav {
    display: none;
  }
  .mobile-menu {
    visibility: visible !important;
    display: block;
  }

}
</style>

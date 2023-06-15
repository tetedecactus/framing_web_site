<template>
  <div class="overflow-hidden">
    <Banner class="" />
    <About />
    <Services />
    <WhyChooseUs />
    <ContactUs />
  </div>
</template>

<script>
import { defineComponent } from "vue";
import Banner from "../components/banner.vue";
import About from "../components/about.vue";
import Services from "../components/services.vue";
import ContactUs from "../components/contactUs.vue";
import WhyChooseUs from "../components/whyChooseUs.vue";

export default defineComponent({
  components: {
    Banner,
    About,
    Services,
    ContactUs,
    WhyChooseUs,
},
});
</script>

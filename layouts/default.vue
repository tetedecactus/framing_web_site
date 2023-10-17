<template>
  <div>
        <Head>
            <Title>East Claw Construction Inc. - Edmonton Framing Labour </Title>
            <Meta name="description" content="My app description"/>
        </Head>
    </div>
  <section>
    <Navbar />
    <div>
      <slot />
    </div>
    <Footer />
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Navbar from "../components/navbar.vue";
import Footer from "../components/footer.vue";

//// import Footer from '@/components/Footer.vue'
export default defineComponent({
  components: {
    Navbar,
    Footer,
  },
});
</script>

<style lang="scss" scoped></style>

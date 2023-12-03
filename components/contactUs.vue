<template>
    <div
      class="bg-contact-us"
    >
      <div class="text-container-contactUs">
        <h2>
          <span>Contact&nbsp;</span> Us
        </h2>
        <p>
          Take advantage of our hassle-free, no-obligation estimates! Just send
          us an email with your name, address, contact number and details of
          your project including any photos, drawings or plans. We'll be in
          touch within 24 hours.
        </p>
        <NuxtLink
          to="/contact"
          class="contact-us-btn"
          >Contact Us Now
        </NuxtLink>
      </div>
      <div class="img-container-contactUs">
        <img
        width="500"
          src="../assets/images/framing_outil.jpg"
          alt="Frey Construction"
        />
      </div>
    </div>
</template>

<style>
.bg-contact-us {
  height: 60vh;
}

.bg-contact-us::before {
  content: "";
  /* background-image: url("../assets/images/frey-cropped.jpg"); */
}

/* @media (max-width: 768px) {
  .bg-frey {
    height: 70vh;
  }

  .bg-frey::before {
    background-position: center center;
  }
} */
</style>

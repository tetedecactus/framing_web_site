<template>
  <div class="page-contact-container">
    <div class="bg-pageContactImg">
      <h2>
        Contact <span>Us</span>
      </h2>
      <div class="contactUs-text-box">
        <p>
          Take advantage of our hassle-free, no-obligation estimates! Just send
          us an email with your name, address, contact number and details of
          your project including any photos, drawings or plans.<span> We'll be in
          touch within 24 hours</span>.
        </p>
      </div>
      <div class="contact-form-box">
        <form @submit.prevent="submitForm" class="max-w-xl mx-auto flex-col relative">
          <div class="mb-4">
            <label
              for="name"
              >Name</label
            >
            <input
              v-model="formData.name"
              type="text"
              id="name"
              name="name"
              placeholder="Your Name"
              required
            />
          </div>
          <div class="mb-4 relative">
            <label
              for="email"
              >Email</label
            >
            <input
              v-model="formData.email"
              type="email"
              id="email"
              name="email"
              placeholder="Your Email"
              required
            />
          </div>
          <div class="mb-4 relative">
            <label
              for="message"
              >Message</label
            >
            <textarea
              v-model="formData.message"
              id="message"
              name="message"
              rows="4"
              placeholder="Your Message"
              required
            ></textarea>
          </div>
          <div class="text-center relative">
            <button
              type="submit"
              class="btn text-white border-2 border-black text-lg font-bold py-2 px-4 rounded-none bg-[#e42b00] hover:text-black ease-in duration-200"
            >
              Sent
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        name: "",
        email: "",
        message: "",
      },
    };
  },
  methods: {
    submitForm() {
      // Ajoutez ici la logique d'envoi du formulaire
      console.log("Message Send", this.formData);
    },
  },
};
</script>

<style>
input[type="text"],
input[type="email"],
textarea {
  resize: vertical;
}


.bg-pageContactImg::before {
  content: "";
  background-image: url("../assets/images/frame_plan.jpg");
}

::-webkit-scrollbar {
    width: 0.1em;
    background-color: #000;

  }
  ::-webkit-scrollbar-thumb {
    background-color: #000000;

  }
</style>

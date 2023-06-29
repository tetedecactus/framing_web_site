<template>
  <div class="container mx-auto px-4 py-8 relative">
    <div class="bg-planImg pr-[-4] border-4 border-black bg-center bg-fixed overflow-hidden "></div>
    <div class="absolute top-0 left-0 right-0 z-10 pt-20">
      <div class="relative justify-start items-center align-center">
        <h2 class="relative text-6xl font-bold text-center mb-8 text-white">Contact <span class="text-[#e42b00]">Us</span></h2>
        <form @submit.prevent="submitForm" class="max-w-xl mx-auto">
          <div class="mb-4">
            <label for="name" class="text-[#e42b00] block text-sm font-bold mb-2">Name</label>
            <input
              v-model="formData.name"
              type="text"
              id="name"
              name="name"
              placeholder="Your Name"
              class="w-full px-3 py-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
              required
            />
          </div>
          <div class="mb-4 relative">
            <label for="email" class="text-[#e42b00] block text-sm font-bold mb-2">Email</label>
            <input
              v-model="formData.email"
              type="email"
              id="email"
              name="email"
              placeholder="Your Email"
              class="w-full px-3 py-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
              required
            />
          </div>
          <div class="mb-4 relative">
            <label for="message" class="text-[#e42b00] block text-sm font-bold mb-2">Message</label>
            <textarea
              v-model="formData.message"
              id="message"
              name="message"
              rows="4"
              placeholder="Your Message"
              class="w-full px-3 py-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
              required
            ></textarea>
          </div>
          <div class="text-center relative">
            <button
              type="submit"
              class="btn text-white border-2 border-black text-lg font-bold py-2 px-4 rounded-none bg-[#e42b00] hover:text-black ml-10 ease-in duration-200"
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
        name: '',
        email: '',
        message: ''
      }
    };
  },
  methods: {
    submitForm() {
      // Ajoutez ici la logique d'envoi du formulaire
      console.log('Message Send', this.formData);
    }
  }
};
</script>

<style>
input[type="text"],
input[type="email"],
textarea {
  resize: vertical;
}

.bg-planImg {
  margin-top: 0;
  padding-right: 0rem !important;
  /* padding: 260px 0 100px 0 !important; */
  position: relative;
  height: 85vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #171717 !important;
  overflow-x: hidden;
}

.bg-planImg::before {
  background-attachment: fixed;
  content: "";
  background-image: url("../assets/images/frame_plan.jpg");
  background-position: top center;
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
  opacity: 40%;
}
</style>

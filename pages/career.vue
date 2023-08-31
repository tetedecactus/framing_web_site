<template>
  <div class="career-container mx-auto flex px-4 py-8 relative items-center">
    <div
      class="bg-planImg pr-[-4] border-4 border-black bg-center bg-fixed overflow-hidden"
    ></div>
    <div class="absolute top-0 left-0 right-0 z-10 pt-20 mb-20">
      <h2 class="relative text-6xl font-bold text-center mb-8 text-white">
        Join our <span class="text-[#e42b00]">TEAM</span>
      </h2>
      <div class="flex flex-row">
        <div
          class="intro relative flex items-center w-1/2 justify-start px-14 pt-20"
        >
          <p class="text-white text-md text-justify">
            Are you seeking
            <span class="text-[#e42b00] font-bold italic"
              >new challenges and opportunities?</span
            >
            Join our
            <span class="text-[#e42b00] font-bold italic">dynamic team</span> of
            framers and embark on an exciting journey in the world of
            framing.<br /><br />
            At our company, we believe in fostering a collaborative and
            growth-oriented environment where each team member can thrive. As a
            framer, you'll have the chance to work on diverse projects, from
            <span class="text-[#e42b00] font-bold italic"
              >commercial installations to residential renovations</span
            >. With our state-of-the-art equipment and industry expertise,
            you'll have all the resources needed to showcase your skills and
            craftsmanship.<br /><br />
            We value creativity, precision, and a passion for delivering
            exceptional results. Whether you're an
            <span class="text-[#e42b00] font-bold italic"
              >experienced framer</span
            >
            or
            <span class="text-[#e42b00] font-bold italic">just starting</span>
            your career in the field, we provide training and mentorship to help
            you expand your knowledge and expertise. Join our team and become
            part of a supportive community that values innovation and
            craftsmanship.<br /><br />
            If you're
            <span class="text-[#e42b00] font-bold italic"
              >ready to take on new challenges</span
            >, explore your potential, and join
            <span class="text-[#e42b00] font-bold italic"
              >a team that values your contributions</span
            >, we invite you to
            <span class="text-[#e42b00] font-bold italic">apply today</span>.
            Together, let's create extraordinary frames and build a rewarding
            career in the art of framing.
          </p>
        </div>
        <div
          class="form w-1/2 relative justify-center items-center px-14 mt-20"
        >
          <form
            @submit.prevent="submitForm"
            class="max-w-xl mx-auto flex-col items-center"
          >
            <div class="mb-4">
              <label
                for="name"
                class="text-[#e42b00] block text-sm font-bold mb-2"
                >Name</label
              >
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
              <label
                for="email"
                class="text-[#e42b00] block text-sm font-bold mb-2"
                >Email</label
              >
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
              <label
                for="message"
                class="text-[#e42b00] block text-sm font-bold mb-2"
                >Message</label
              >
              <textarea
                v-model="formData.message"
                id="message"
                name="message"
                rows="4"
                placeholder="Your Message"
                class="w-full h-64 px-3 py-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
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

.bg-planImg {
  margin-top: 0;
  padding-right: 0rem !important;
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
  opacity: 35%;
}

.intro {
  justify-items: center !important;
}

.form {
  justify-items: center !important;
  justify-content: center !important;
}
</style>

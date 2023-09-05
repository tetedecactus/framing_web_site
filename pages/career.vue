<template>
  <div class="career-container">
    <div class="bg-pageCareerImg">
      <div>
        <h2>
          Join our <span>TEAM</span>
        </h2>
        <div class="career-subcontainer">
          <div class="career-text-box">
            <p>
              Are you seeking
              <span>new challenges and opportunities?</span
              >
              Join our
              <span>dynamic team</span> of
              framers and embark on an exciting journey in the world of
              framing.<br /><br />
              At our company, we believe in fostering a collaborative and
              growth-oriented environment where each team member can thrive. As a
              framer, you'll have the chance to work on diverse projects, from
              <span>commercial installations to residential renovations</span
              >. With our state-of-the-art equipment and industry expertise,
              you'll have all the resources needed to showcase your skills and
              craftsmanship.<br /><br />
              We value creativity, precision, and a passion for delivering
              exceptional results. Whether you're an
              <span>experienced framer</span
              >
              or
              <span>just starting</span>
              your career in the field, we provide training and mentorship to help
              you expand your knowledge and expertise. Join our team and become
              part of a supportive community that values innovation and
              craftsmanship.<br /><br />
              If you're
              <span>ready to take on new challenges</span>, explore your potential, and join
              <span>a team that values your contributions</span>, we invite you to
              <span>apply today</span>.
              Together, let's create extraordinary frames and build a rewarding
              career in the art of framing.
            </p>
          </div>
          <div class="career-form-box">
            <form
              @submit.prevent="submitForm"
              class="max-w-xl mx-auto flex-col"
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

.bg-pageCareerImg::before {
  content: "";
  background-image: url("../assets/images/frame_plan.jpg");
 
}

</style>

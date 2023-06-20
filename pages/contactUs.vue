<template>
  <div class="container mx-auto px-4 py-8">
    <h2 class="text-3xl font-bold text-center mb-8">Contactez-nous</h2>
    <form @submit.prevent="submitForm" class="max-w-md mx-auto">
      <div class="mb-4">
        <label for="name" class="block text-sm font-bold mb-2">Nom</label>
        <input
          v-model="formData.name"
          type="text"
          id="name"
          name="name"
          placeholder="Entrez votre nom"
          class="w-full px-3 py-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
          required
        />
      </div>
      <div class="mb-4">
        <label for="email" class="block text-sm font-bold mb-2">Email</label>
        <input
          v-model="formData.email"
          type="email"
          id="email"
          name="email"
          placeholder="Entrez votre adresse email"
          class="w-full px-3 py-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
          required
        />
      </div>
      <div class="mb-4">
        <label for="message" class="block text-sm font-bold mb-2">Message</label>
        <textarea
          v-model="formData.message"
          id="message"
          name="message"
          rows="4"
          placeholder="Entrez votre message"
          class="w-full px-3 py-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
          required
        ></textarea>
      </div>
      <div class="text-center">
        <button
          type="submit"
          class="btn bg-indigo-500 hover:bg-indigo-600 text-white px-4 py-2 rounded"
        >
          Envoyer
        </button>
      </div>
    </form>
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
      console.log('Formulaire soumis', this.formData);
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
</style>

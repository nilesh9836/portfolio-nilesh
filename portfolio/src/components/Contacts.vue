<template>
  
    <v-form @submit.prevent="submitForm">
    <label>
      Name:
      <v-text-field type="text" v-model="formData.name" required />
    </label>
    <label>
      Email:
      <v-text-field type="email" v-model="formData.email" required />
    </label>
    <label>
      Message:
      <v-textarea v-model="formData.message" required></v-textarea>
    </label>
    <v-btn type="submit">Send</v-btn>
  </v-form>
</template>

<script>
export default {
  name: "ContactForm",
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
      // Send a request to the server with the form data
      // Or, you can use a library like axios to make the request
      // axios.post('/api/contact', this.formData)
      // .then(response => { /* handle success */ })
      // .catch(error => { /* handle error */ })
      console.log(this.formData);
    },
  },
};
</script>

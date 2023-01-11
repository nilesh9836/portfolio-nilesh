<template>
  <form @submit.prevent="submitForm">
    <label>
      Name:
      <input type="text" v-model="formData.name" required />
    </label>
    <label>
      Email:
      <input type="email" v-model="formData.email" required />
    </label>
    <label>
      Message:
      <textarea v-model="formData.message" required></textarea>
    </label>
    <button type="submit">Send</button>
  </form>
</template>

<script>
export default {
  name: 'ContactForm',
  data() {
    return {
      formData: {
        name: '',
        email: '',
        message: ''
      }
    }
  },
  methods: {
    submitForm() {
      // Send a request to the server with the form data
      // Or, you can use a library like axios to make the request
      // axios.post('/api/contact', this.formData)
      // .then(response => { /* handle success */ })
      // .catch(error => { /* handle error */ })
      console.log(this.formData)
    }
  }
}
</script>

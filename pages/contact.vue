<template>
  <div class="contact-page">
    <section class="contact-section">
      <h2>Contact Me</h2>
      <p>Please feel free to reach out...</p>

      <div class="contact-details">
        <p>Phone: [Your Phone Number]</p>
        <p>Email: [Your Email Address]</p>
        <p>Location: [Your Address or Service Area]</p>
      </div>

      <form @submit.prevent="handleSubmit" class="contact-form">
        <div class="form-group">
          <label for="name">Name:</label>
          <input type="text" id="name" v-model="formData.name" required>
        </div>
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email" v-model="formData.email" required>
        </div>
        <div class="form-group">
          <label for="message">Message:</label>
          <textarea id="message" v-model="formData.message" required></textarea>
        </div>
        <button type="submit" class="submit-button">Send Message</button>
      </form>

      <div class="map-container">
        </div>
    </section>
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
    handleSubmit() {
      // **Handle form submission here**
      // For Netlify Forms, you'll need to add a 'netlify' attribute to your form
      // and potentially a hidden input field. Netlify will then handle submissions.
      // Example using Netlify Forms:
      // 1. Add `data-netlify="true"` to your <form> tag
      // 2. Add a hidden input: `<input type="hidden" name="form-name" value="contact" />`
      // 3. Netlify documentation for more details: https://docs.netlify.com/forms/setup/

      console.log('Form submitted:', this.formData);
      alert('Thank you for your message! We will get back to you shortly.');
      // Reset form
      this.formData = { name: '', email: '', message: '' };
    }
  }
}
</script>

<style scoped>
.contact-section {
  padding: 40px 20px;
  max-width: 700px; /* Limit width for readability */
  margin: 0 auto;
}

.contact-details {
    margin-bottom: 30px;
    text-align: center;
}

.contact-form .form-group {
  margin-bottom: 15px;
}

.contact-form label {
  display: block;
  margin-bottom: 5px;
  font-weight: bold;
}

.contact-form input,
.contact-form textarea {
  width: calc(100% - 22px); /* Adjust for padding and border */
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

.submit-button {
  display: inline-block;
  background-color: #4a90e2; /* Use your calming colors */
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 1rem;
  margin-top: 15px;
}

 .submit-button:hover {
  background-color: #357ABD;
}
</style>

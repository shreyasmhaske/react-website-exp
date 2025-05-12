<template>
  <div class="about-page">
    <section class="about-section">
      <h2>About Me</h2>
      <img src="/images/your-headshot.jpg" alt="Your Name" class="counselor-image" /> <div class="about-content">
        <p>Share your journey, passion, credentials, and therapeutic approach...</p>
        </div>
    </section>

    <section class="testimonials-section">
      <h3>What Clients Say</h3>
      <div class="testimonial">
        <p>"A placeholder testimonial..."</p>
        <p>- Client Name</p>
      </div>
      </section>
  </div>
</template>

<script>
export default {
  // ...
}
</script>

<style scoped>
.about-section {
  padding: 40px 20px;
  text-align: center;
}

.counselor-image {
  width: 150px; /* Adjust size */
  height: 150px; /* Adjust size */
  border-radius: 50%; /* Make it round */
  object-fit: cover;
  margin-bottom: 20px;
}

.about-content {
    max-width: 800px; /* Limit content width for readability */
    margin: 0 auto;
    text-align: left;
}

.testimonials-section {
  padding: 40px 20px;
  background-color: #d1e7dd; /* Use your calming colors */
  text-align: center;
}

.testimonial {
    margin: 20px auto;
    padding: 20px;
    border: 1px solid #ccc;
    max-width: 600px;
    font-style: italic;
}
</style>

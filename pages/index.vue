<template>
  <div class="home-page">
    <section class="hero-section">
      <img src="/images/calming-hero.jpg" alt="Calming scene" /> <h1>Welcome to Your Counseling Practice</h1>
      <p>Finding support for your mental well-being.</p>
      <NuxtLink to="/services" class="cta-button">Learn More About How I Can Help</NuxtLink>
    </section>

    <section class="intro-section">
      <h2>Taking the First Step Towards Healing</h2>
      <p>Provide a brief, empathetic introduction...</p>
      </section>

    <section class="quick-links">
       <h3>Quick Links</h3>
       <ul>
         <li><NuxtLink to="/about">Meet Your Counselor</NuxtLink></li>
         <li><NuxtLink to="/contact">Contact Me</NuxtLink></li>
       </ul>
    </section>
  </div>
</template>

<script>
export default {
  // Page specific JavaScript options
}
</script>

<style scoped>
/* Page specific styles using scoped CSS */
.hero-section {
  position: relative;
  text-align: center;
  color: white; /* Text color over the image */
  padding: 100px 20px; /* Adjust padding as needed */
  background-image: url('/images/calming-hero.jpg'); /* Ensure path is correct */
  background-size: cover;
  background-position: center;
  /* Add overlay or text shadow for readability */
}

.hero-section h1, .hero-section p {
   text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
}


.intro-section {
  padding: 40px 20px;
  text-align: center;
  background-color: #e2f0cb; /* Use your calming colors */
}

 .cta-button {
  display: inline-block;
  background-color: #4a90e2; /* Use your calming colors */
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  text-decoration: none; /* Remove underline from NuxtLink */
  font-size: 1rem;
  margin-top: 15px;
}

.cta-button:hover {
  background-color: #357ABD;
}

.quick-links {
    text-align: center;
    padding: 20px;
}
</style>

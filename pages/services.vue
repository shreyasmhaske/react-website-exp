<template>
  <div class="services-page">
    <section class="services-section">
      <h2>Our Services</h2>
      <div class="service-list">
        <div class="service-item">
          <h3>Individual Therapy</h3>
          <p>Describe your individual therapy services...</p>
        </div>
        <div class="service-item">
          <h3>Couples Counseling</h3>
          <p>Describe your couples counseling services...</p>
        </div>
        <div class="service-item">
          <h3>[Your Specialty]</h3>
          <p>Detail your expertise...</p>
        </div>
      </div>
    </section>

    <section class="fees-insurance-section">
      <h3>Fees and Insurance</h3>
      <p>Provide clear information about fees, insurance, and sliding scale...</p>
    </section>
  </div>
</template>

<script>
export default {
  // ...
}
</script>

<style scoped>
.services-section, .fees-insurance-section {
  padding: 40px 20px;
}

.service-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); /* Responsive grid */
    gap: 20px;
    margin-top: 30px;
}

.service-item {
    border: 1px solid #eee;
    padding: 20px;
    border-radius: 5px;
    background-color: white; /* Card background */
    box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
}

.service-item h3 {
    color: #4a90e2; /* Highlight color for headings */
}
</style>

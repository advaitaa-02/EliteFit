<template>
    <div class="testimonials">
      <h2>Testimonials</h2>
      <div class="image-row">
        <img src="@/images/Alex.png" alt="Testimonial 1">
        <img src="@/images/Emily.png" alt="Testimonial 2">
        <img src="@/images/David.png" alt="Testimonial 3">
        <img src="@/images/Lisa.png" alt="Testimonial 4">
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Testimonials'
  };
  </script>
  
  <style scoped>
  /* Add styles for the Testimonials component */
  .testimonials {
    text-align: center;
    padding: 20px;
  }
  
  .testimonials h2 {
    font-size: 24px;
    margin-bottom: 20px;
  }
  
  .image-row {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
  }
  
  .image-row img {
    width: 200px; /* Adjust the width as needed */
    height: auto; /* Maintain aspect ratio */
  }
  </style>
  
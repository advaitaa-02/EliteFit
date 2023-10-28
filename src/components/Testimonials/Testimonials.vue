<template>
    <div class="testimonials">
      <h2>Testimonials</h2>
      <div class="image-row">
        <div class="image">
            <img src="@/images/Alex.png" alt="Testimonial 1">
            <div class="overlay"></div>
        </div>
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
  .image-row .image {
    opacity: none;
  }

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

  .image-row img:hover {
    opacity: 0.9;
  }
  </style>
  
<script setup>
import NavBar from './components/NavBar/NavBar.vue'
import ImageGrid from './components/ImageGrid/ImageGrid.vue'
import About from './components/About/About.vue'
import Testimonials from './components/Testimonials/Testimonials.vue'
import Footer from './components/Footer/Footer.vue'
</script>

<template>
  <header>
      <button class="feedback-button">Feedback</button>
      <NavBar />
      <ImageGrid />
      <About />
      <Testimonials />
      <Footer />
  </header>

  <main>
    
  </main>
</template>

<style scoped>
/* header {
  line-height: 1.5;
} */


.feedback-button {
  position: fixed;
  width: 28px;
  height: 79px;
  top: 353px;
  right: -25px;
  padding: 6px 7px 6px 6px;
  border: 2px solid #000;
  background-color: white;
  color: black;
  border-radius: 5px;
  cursor: pointer;
  transform: rotate(270deg);
  width: 80px; /* Set the width */
  height: 28px; 
  padding: 0px 10px;
  /* height: 15px; Set the height */
}

</style>

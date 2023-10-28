<template>
  <div class="about-container">
    <div class="about-image">
      <img src="@/images/aunty.png" alt="Aunty Image">
    </div>
    <div class="about-text">
      <h2>ABOUT PISTONS</h2>
      <p>
        Established in 1897, our beloved fountain pen haven, 'PISTONS, has been a haven for pen enthusiasts for generations. With a century-long dedication to fine writing instruments, we've bridged tradition and modernity, offering a curated selection of vintage and contemporary fountain pens. Our little shop, nestled in the heart of town, continues to inspire a love for the art of writing, connecting past and present through the timeless elegance of ink on paper.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style scoped>
.about-container {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 20px;
}

.about-image {
  flex: 1;
  text-align: center;
  width: 597px;
height: 450px;
top: 93px;
left: 61px;
padding: 0px, 30px, 0px, 30px;

}

.about-image img {
  max-width: 100%;
  height: auto;
}

.about-text {
  flex: 1;
  padding: 20px;
  text-align: left;
}

.about-text h2 {
  font-size: 24px;
}

.about-text p {
  font-size: 16px;
}
</style>

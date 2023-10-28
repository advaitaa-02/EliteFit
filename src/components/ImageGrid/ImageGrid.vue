<template>
  <div>
    <div class="image-grid">
      <img src="@/images/image1.jpg" alt="Image 1" class="image-standard">
      <img src="@/images/image2.jpg" alt="Image 2" class="image-standard">
    </div>
    <div class="image-grid">
      <img src="@/images/image3.jpg" alt="Image 3" class="image-standard">
      <img src="@/images/image4.jpg" alt="Image 4" class="image-standard">
    </div>
    <div class="image-grid">
      <img src="@/images/image5.jpg" alt="Image 5" class="image-standard">
      <img src="@/images/image6.jpg" alt="Image 6" class="image-standard">
    </div>
    <div class="image-grid">
      <img src="@/images/image7.jpg" alt="Image 7" class="image-special">
    </div>
  </div>
</template>

<style scoped>
/* Basic styles for the image grid */
.image-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

/* Styles for standard images */
.image-standard {
  width: 100%;
}

/* Style for the 7th image */
.image-special {
  width: 200%;
  height: 599px;
  top: 1921px;

}
</style>

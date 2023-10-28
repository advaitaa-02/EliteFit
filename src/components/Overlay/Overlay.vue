<template>
  <div v-if="isOpen" class="overlay">
    <div class="overlay-content">
      <!-- Content for the overlay -->
      <button @click="closeOverlay">Close</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    openOverlay() {
      this.isOpen = true;
    },
    closeOverlay() {
      this.isOpen = false;
    },
  },
};
</script>

<style scoped>
.overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 999;
}

.overlay-content {
  background: white;
  padding: 20px;
  border-radius: 5px;
}
</style>

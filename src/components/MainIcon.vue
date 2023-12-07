<template>
  <div>
    <img :class="['spinning-top', { 'paused': !isHovered }]" @mouseover="startSpinning" @mouseout="stopSpinning" src="MainIcon.svg" alt="Icon">
  </div>
</template>

<script>
export default {
  data() {
    return {
      isHovered: false
    };
  },
  methods: {
    startSpinning() {
      this.isHovered = true;
    },
    stopSpinning() {
      this.isHovered = false;
    }
  }
};
</script>

<style scoped>
@keyframes spin {
  0% { transform: rotateY(0deg); }
  100% { transform: rotateY(360deg); }
}

.spinning-top {
  width: 200px; /* Set the width of your image */
  height: 200px; /* Set the height of your image */
  border-radius: 50%; /* Make the border-radius 50% to create a circle */
  object-fit: cover; /* Ensure the image covers the entire container */
  animation: spin 3s infinite linear; /* Adjusted the duration to 3 seconds for a faster spin */
}

.paused {
  animation-play-state: paused; /* Pause the animation when the 'paused' class is present */
}
</style>

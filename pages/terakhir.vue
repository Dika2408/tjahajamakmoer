<template>
  <div class="thank-you-container d-flex align-items-center justify-content-center">
    <div class="text-center">
      <!-- Coffee logo placeholder -->
      <div class="coffee-logo mb-3">
        <img src="https://via.placeholder.com/100" alt="Coffee Logo" class="img-fluid">
      </div>
      <!-- Thank You Message -->
      <h2 class="text-white">THANKS YOU!</h2>
      <p class="text-white">you have placed your order successfully :)</p>
      <!-- Button -->
      <button class="btn btn-light mt-3" @click="goBack">Back to Home</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ThankYou',
  methods: {
    goBack() {
      // Logic to go back to home, e.g., using vue-router
      this.$router.push('/');
    }
  }
};
</script>

<style scoped>
.thank-you-container {
  height: 100vh;
  background-image: url('assets/img/download3.jpeg'); /* Replace with your coffee beans image */
  background-size: cover;
  background-position: center;
}

.coffee-logo img {
  width: 80px;
  height: 80px;
}

h2, p {
  font-family: 'Arial', sans-serif;
}

p {
  font-size: 1.1rem;
}

.btn-light {
  border-radius: 20px;
}
</style>

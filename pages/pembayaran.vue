<template>
    <div class="row justify-content-end">
        <div class="col-4">
          <NuxtLink to="../" class="btn btn-warning">BACK</NuxtLink>
        </div>
    </div>
  <div class="card" style="width: 25rem">
    <img src="assets/img/download1.jpeg" class="img-thumbnail" alt="Coffee Image">
    <div class="card-body">
      <h5 class="card-title">Descriptions</h5>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <p class="card-text">
        GOOD DAY
      </p>
      <div class="d-flex justify-content-between align-items-center">
        <div>
        </div>
        <div class="price">
          <strong>Rp. 20.000</strong>
        </div>
      </div>
      <NuxtLink to="/terakhir">
      <a href="#" class="btn btn-success btn-block mt-3">Pay Now</a>
    </NuxtLink>
      
    </div>
  </div>
</template>

<script>
export default {
  name: 'CoffeeCard',
};
</script>

<style scoped>
.card {
  border-radius: 10px;
  overflow: hidden;
}
.card-img-top {
  border-radius: 0;
}
.price {
  font-size: 1,2em;
}
</style>

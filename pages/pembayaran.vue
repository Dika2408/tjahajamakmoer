<template>
    <div class="row">
        <div class="col-2">
          <NuxtLink to="../" class="btn btn-success">BACK</NuxtLink>
        </div>
        <div class="d-flex-end col-5">
          <NuxtLink to="terakhir" class="btn btn-success ">NEXT</NuxtLink>
        </div>
      
    </div>
  <div class="card" style="width: 15rem">
    <img src="assets/img/download1.jpeg" class="img-thumbnail" alt="Coffee Image">
    <div class="card-body">
      <h5 class="card-title">Cappucino</h5>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <p class="card-text">
        minuman kopi panas berbahan dasar espresso yang dibuat dengan lapisan espresso, susu kukus, dan busa susu di atasnya.
      </p>
      <div class="d-flex justify-content-between align-items-center">
        <div>
        </div>
        <div class="price">
          <strong>Rp. 20.000</strong>
        </div>
      </div>
      <nuxt-link href="https://wa.me/62" class=" btn btn-success btn-block mt-5 bi bi-whatsapp">Order wa</nuxt-link>
    </div>
  </div>
  <div class="card" style="width: 15rem">
    <img src="assets/img/download5.jpeg" class="img-thumbnail" alt="Coffee Image">
    <div class="card-body">
      <h5 class="card-title">Americano</h5>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <p class="card-text">
        Espresso dan air panas sepertinya resep sederhana. Namun pada kenyataannya, kualitas bahan dan cara pencampurannya akan menentukan apakah sebuah Americano disiapkan dengan benar.
      </p>
      <div class="d-flex justify-content-between align-items-center">
        <div>
        </div>
        <div class="price">
          <strong>Rp. 20.000</strong>
        </div>
      </div>
        <nuxt-link href="https://wa.me/62" class=" btn btn-success btn-block mt-5 bi bi-whatsapp">Order wa</nuxt-link>
    </div>
  </div>
  <div class="card" style="width: 15rem">
    <img src="assets/img/download6.jpeg" class="img-thumbnail" alt="Coffee Image">
    <div class="card-body">
      <h5 class="card-title">Pisang Goreng</h5>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <p class="card-text">
        Pisang goreng adalah pisang yang di goreng dengan adanya campuran tepung terigu.
      </p>
      <div class="d-flex justify-content-between align-items-center">
        <div>
        </div>
        <div class="price">
          <strong>Rp. 20.000</strong>
        </div>
      </div>
      <nuxt-link href="https://wa.me/62" class=" btn btn-success btn-block mt-5 bi bi-whatsapp">Order wa</nuxt-link>
    </div>
  </div>
  <div class="card" style="width: 15rem">
    <img src="assets/img/download7.jpeg" class="img-thumbnail" alt="Coffee Image">
    <div class="card-body">
      <h5 class="card-title">nasi goreng</h5>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <p class="card-text">
      Nasi goreng makanan berupa nasi yang digoreng dan dicampur dalam minyak goreng, margarin, atau mentega.
      </p>
      <div class="d-flex justify-content-between align-items-center">
        <div>
        </div>
        <div class="price">
          <strong>Rp. 20.000</strong>
        </div>
      </div>
      <nuxt-link href="https://wa.me/62 " class=" btn btn-success btn-block mt-5 bi bi-whatsapp">Order wa</nuxt-link>
    </div>
  </div>
  <div class="card" style="width: 15rem">
    <img src="assets/img/download8.jpeg" class="img-thumbnail" alt="Coffee Image">
    <div class="card-body">
      <h5 class="card-title">Kentang Goreng</h5>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <i class="bi bi-star-fill text-warning"></i>
      <p class="card-text">
        hidangan yang dibuat dari potongan-potongan kentang yang digoreng dalam minyak goreng panas.
      </p>
      <div class="d-flex justify-content-between align-items-center">
        <div>
        </div>
        <div class="price">
          <strong>Rp. 20.000</strong>
        </div>
      </div>
      <nuxt-link href="https://wa.me/62" class=" btn btn-success btn-block mt-5 bi bi-whatsapp">ORDER VIA WA</nuxt-link>
      <nuxt-link href="https://www.instagram.com/warkop.tjahajamakmoer/" class=" btn btn-danger btn-block mt-5 bi bi-instagram">ORDER VIA IG</nuxt-link>
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

<template>
<div>
    <div class="row justify-content-end">
        <div class="col-4">
          <NuxtLink to="../" class="btn btn-danger">BACK</NuxtLink>
        </div>
    </div>
    <img src="assets/img/download2.jpeg" class="img-thumbnail" alt="150" width="500rem">
    <div class="container text-center">
      <div class="row ">
        <div class="col">
          Hot Coffe
        </div>
        <div class="col">
          Cold Coffe
        </div>
        <div class="col">
          Others
        </div>
      </div>
    </div>
</div>
  
      <div class="row gap-3 justify-content-center">
        <div class="col-10">
          <div class="input-group mb-3">
            <button class="btn btn-outline-secondary" type="button" id="button-addon1"><i class="bi bi-search"></i></button>
            <input type="text" class="form-control" placeholder="" aria-label="Example text with button addon" aria-describedby="button-addon1">
          </div>
        </div>
        
      </div>
      
  
    <ul v-for="item in items" :key="item.id">
      <li>{{ item.nama }}</li>
    </ul>
    <ol class="list-group list-group-numbered">
  <li class="list-group-item d-flex justify-content-between align-items-start">
    <div class="ms-2 me-auto">
      <div class="fw-bold">Americano</div>
      RP:20000
    </div>
    <NuxtLink to="/pembayaran">
      <span class="badge text-bg-danger rounded-pill"><i class="bi bi-plus-square-fill"></i></span>
    </NuxtLink>
  </li>
  <li class="list-group-item d-flex justify-content-between align-items-start">
    <div class="ms-2 me-auto">
      <div class="fw-bold">Cappucino</div>
      RP.20000
    </div>
    <NuxtLink to="/pembayaran">
      <span class="badge text-bg-danger rounded-pill"><i class="bi bi-plus-square-fill"></i></span>
    </NuxtLink>
  </li>
  <li class="list-group-item d-flex justify-content-between align-items-start">
    <div class="ms-2 me-auto">
      <div class="fw-bold">Pisang Goreng</div>
      RP.20000
    </div>
    <NuxtLink to="/pembayaran">
      <span class="badge text-bg-danger rounded-pill"><i class="bi bi-plus-square-fill"></i></span>
    </NuxtLink>
  </li>
  <li class="list-group-item d-flex justify-content-between align-items-start">
    <div class="ms-2 me-auto">
      <div class="fw-bold">Nasi Goreng</div>
      Rp.20000
    </div>
    <NuxtLink to="/pembayaran">
      <span class="badge text-bg-danger rounded-pill"><i class="bi bi-plus-square-fill"></i></span>
    </NuxtLink>
  </li>
</ol>
  
</template>


<script setup>
const supabase = useSupabaseClient()
const items = ref([])

async function getProduk() {
  let { data, error } = await supabase
  .from('produk')
  .select('*')
  if(data) {
    items.value = data
  }
}

onMounted(() => getProduk())
</script>

<style scoped>

</style>
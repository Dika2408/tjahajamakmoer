<template>
<div>
  <div class="row justify-content-end">
    <nuxt-link href="https://wa.me/62" class=" text-success bi bi-headset">COSTUMER SERVICE</nuxt-link>
        <div class="col-3">
          <NuxtLink to="../" class="btn btn-success">BACK</NuxtLink>
        </div>
    </div>
    <img src="assets/img/download2.jpeg" class="img-thumbnail" alt="150" width="500rem">
    <div class="container text-center bg-info">
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
    <div class="row gap-3 justify-content-center">
        <div class="col-10">
          <div class="input-group mb-3">
            <button class="btn btn-outline-secondary" type="button" id="button-addon1"><i class="bi bi-search"></i></button>
            <form @submit.prevent="getProduk" class="row pt-5 d-flex justify-content-center">
                    <div class="col-lg-10">
                        <input v-model="keyword" type="search" class="form-control form-control-md rounded-5" name="cari-produk" id="cari-produk" placeholder="Mau pesank apa hari ini?" autocomplete="off">
                    </div>
                </form>
          </div>
        </div>
      </div>
    <div class="container">
      <div class="row" v-for="item in items" :key="item.id">
        <div class="card mb-2" style="width: 15rem">
          <img :src="item.foto" class="img-thumbnail" alt="Coffee Image">
          <div class="card-body">
            <h5 class="card-title">{{ item.nama }}</h5>
            <i class="bi bi-star-fill text-warning"></i>
            <i class="bi bi-star-fill text-warning"></i>
            <i class="bi bi-star-fill text-warning"></i>
            <i class="bi bi-star-fill text-warning"></i>
            <i class="bi bi-star-fill text-warning"></i>
            <p class="card-text">
              {{ item.deskripsi}}
            </p>
            <div class="d-flex justify-content-between align-items-center">
              <div>
              </div>
              <div class="price">
                <strong>Rp. {{ item.harga }}</strong>
              </div>
            </div>
            <nuxt-link href="https://wa.me/62" class=" btn btn-success btn-block mt-5 bi bi-whatsapp">Order wa</nuxt-link>
          </div>
        </div>
       
      </div> 
    </div> 
</div>
  
      
    
</template>


<script setup>
const supabase = useSupabaseClient()
const items = ref([])

async function getProduk() {
  let { data, error } = await supabase
  .from('produk')
  .select()
  if(data) {
    items.value = data
  }
}

onMounted(() => getProduk())
</script>

<style scoped>

</style>
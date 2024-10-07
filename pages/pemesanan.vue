<template>
  <div>
    <h1>Hot Coffee</h1>
    <h1>Cold Coffee</h1>
    <h1>Others</h1>

    <ul v-for="item in items" :key="item.id">
      <li>{{ item.nama }}</li>
    </ul>
  </div>
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

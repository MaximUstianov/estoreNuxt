<template>
  <no-ssr v-pin="{padding: {top: 20}}" class="border-right filter-form">
  <b-form>
    <b-form-group label="Brand:">
      <b-form-select v-model="selectedBrand" :options="brands"></b-form-select>
    </b-form-group>
    <b-form-group label="Model:">
      <b-form-select v-model="selectedBrand" :options="brands"></b-form-select>
    </b-form-group>
  </b-form>
  </no-ssr>
</template>

<script>
  export default {
    name: "CatalogFilter",
    data(){
      return{
        selectedBrand : '',
        brands : [{ value: 'bmw', text: 'BMW' },
          { value: 'Yamaha', text: 'Yamaha' },
          { value: 'PSJ-Yamaha', text: 'psjjj-400' }
        ]
      }
    }
  }
</script>

<style scoped>
.filter-form{
  padding-right: 10px;
  position: sticky;
  height: 100vh;
}
</style>

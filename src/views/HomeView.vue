<template>
  <div class="home">
    <v-autocomplete
      clearable
      label="Autocomplete"
      class="selectCity"
      :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
      variant="solo"
    ></v-autocomplete>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .home{
    max-width: 1000px;
    height: max-content;
    margin: auto;
    padding: 20px;
    background-color: white;
  }

  .selectCity {
    width: 200px;
  }
</style>
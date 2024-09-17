<script>
export default {
  data() {
    return {
      
    }
  },
  props: {
    cardImage: {
        type: String,
        required: true,
    },
    cardPrice: {
        type: String,
        required: false,
    },
    cardSeries: {
        type: String,
        required: true,
    },
    cardType: {
        type: String,
        required: false,
    },
  }
}
</script>

<template>
<div class="card">
    <img :src="cardImage" :alt="cardSeries">
</div>
<h3>{{ cardSeries }}</h3>
</template>

<style scoped>
</style>
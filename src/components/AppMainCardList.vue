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
<article class="card">
   <a href="#"> <img :src="cardImage" :alt="cardSeries"></a>
    <p>{{ cardSeries }}</p>
</article>
</template>

<style lang="scss" scoped>
.card {
 width:calc(100vw / 10 - 1rem);
  p {
    margin-top: 1.5rem;
    font-size: 12px;
    font-weight: 600;
    color: #fff;
    text-transform: uppercase;
    }
}
img {
    width: 100%;
    object-fit: fill;
    object-position: center;
    height: calc(100vw/10 - 1rem);
}
</style>
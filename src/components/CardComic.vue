<script>
export default {

  // Definisco le Proprieta' che il Componente Card deve ricevere dal Componente Padre
  props: {

    thumb: {
      type: String,
      required: true
    },

    series: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <div class="card">
    <img :src="thumb">

    <span>{{ series }}</span>
  </div>
</template>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  gap: 10px;

  img {
    aspect-ratio: 1/1;
    object-fit: cover;
    object-position: top;
    display: block;
  }

  span {
    text-transform: uppercase;
  }
}
</style>
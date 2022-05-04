<template>
  <div class="col-2">
    <div class="card">
      <div class="img_card">
        <img :src="thumb" alt="" />
      </div>
      <div class="text_card">
        <p>{{ series }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "fumettiCardComponent",
  props: {
    thumb: String,
    series: String,
  },
};
</script>

<style lang="scss" scoped>


.card {
    padding: 0.75rem;

    .img_card {
      img {
        aspect-ratio: 1/1;
        object-fit: cover;
        object-position: top;
      }
    }

    .text_card {
      p {
        text-transform: uppercase;
        padding-top: 1rem;
      }
    }
  }
</style>


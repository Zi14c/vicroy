<script>
import Rating from "./Rating.vue";

export default {
  props: {
    data: Object,
  },
  components: {
    Rating,
  },
};
</script>
<template>
  <div class="card mb-3" style="max-width: 540px">
    <div class="row no-gutters">
      <div class="col-md-4">
        <img :src="data.imageUrl" class="card-img" alt="..." />
      </div>
      <div class="col-md-8">
        <div class="card-body">
          <h5 class="card-title">{{ data.productName }}</h5>
          <Rating :initalRating="data.rating" />
          <p class="card-text">{{ data.description }}</p>
          <p class="card-text">
            <small class="text-muted">{{ data.releasedDate }}</small>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style>  
.card-title {
  font-size: 30;
}

.card-text {
  font-size:2,5;
}

.card-img {
  max-width: 100%;
  height: auto;
  margin-bottom: 1rem;
}
</style>
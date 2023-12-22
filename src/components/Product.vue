<script>
import Rating from "./Rating.vue";
import Buy from "./Buy.vue";

export default {
  props: {
    data: Object,
  },
  components: {
    Rating,
    Buy,
  },
};
</script>

<template>
  <div class="card mb-3" style="max-width: 540px">
    <div class="row no-gutters">
      <div class="col-md-4 d-flex align-items-center">
        <img :src="data.imageUrl" class="card-img" alt="..." />
      </div>
      <div class="col-md-8">
        <div class="card-body">
          <h5 class="card-title">{{ data.productName }}</h5>
          <Rating :initialRating="data.rating"/>
          <p class="card-text"></p>
          <p class="card-text">{{ data.price }}</p>
          <p class="card-text">{{ data.description }}</p>
          <Buy/>
          <p class="card-text">
            <small class="text-muted">{{ data.releasedDate }}</small>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

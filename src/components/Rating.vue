<script>
  export default {
    props: ['initialRating'],
    data() {
      return {
        rating: this.initialRating,
        color: 'red'
      }
    },
    methods: {
      assignRating(newRating) {
        this.rating = newRating
      }
    }
  }
</script>

<template>
  <div>
    <p>Bewertung: {{ rating }}</p>
    <span :style="{ color: color }" v-on:click="assignRating(1)">
      <i v-if="rating >= 1" class="bi bi-heart-fill"></i>
      <i v-else class="bi bi-heart text-black"></i>
    </span>
    <span :style="{ color: color }" v-on:click="assignRating(2)">
      <i v-if="rating >= 2" class="bi bi-heart-fill"></i>
      <i v-else class="bi bi-heart text-black"></i>
    </span>
    <span :style="{ color: color }" v-on:click="assignRating(3)">
      <i v-if="rating >= 3" class="bi bi-heart-fill"></i>
      <i v-else class="bi bi-heart text-black"></i>
    </span>
    <span :style="{ color: color }" v-on:click="assignRating(4)">
      <i v-if="rating >= 4" class="bi bi-heart-fill"></i>
      <i v-else class="bi bi-heart text-black"></i>
    </span>
    <span :style="{ color: color }" v-on:click="assignRating(5)">
      <i v-if="rating >= 5" class="bi bi-heart-fill"></i>
      <i v-else class="bi bi-heart text-black"></i>
    </span>
  </div>
</template>
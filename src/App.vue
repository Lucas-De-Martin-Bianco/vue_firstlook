<script>
  import Rating from './components/Rating.vue';

  export default {
    components: {
      Rating
    }
  }
</script>

<template>
  <div>
    <Rating initialRating='1' />
    <Rating initialRating='2' />
    <Rating initialRating='3' />
    <Rating initialRating='4' />
    <Rating initialRating='5' />
  </div>
</template>
<script>
  export default {
    data() {
      return {
        bought: false,
      };
    },
    computed: {
      buttonText() {
        return this.bought ? 'Bought' : 'Buy';
      },
    },
    methods: {
      handleBuyClick() {
        if (!this.bought) {
          this.bought = true;
        }
      },
    },
  };
</script>

<template>
    <div>
      <button
        :class="{ 'btn-warning': !bought, 'btn-success': bought }"
        @click="handleBuyClick"
        :disabled="bought"
        class="btn"
      >
        {{ buttonText }}
      </button>
    </div>
</template>

<style>
  .btn-success {
    background-color: green;
    color: white;
  }
  .btn-warning {
    background-color: yellow;
    color: black;
  }
</style>
  
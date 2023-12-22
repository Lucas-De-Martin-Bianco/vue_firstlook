<script>
import Product from "./Product.vue";

export default {
  components: {
    Product,
  },
  data() {
    return {
      products: [
        {
          id: "1",
          imageUrl: "http://www.gunshopschweiz.ch/Product/Show/6442",
          productName: "Taurus Raging Bull (2-454089M)",
          price: "1231.-",
          releasedDate: "May 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 4,
        },
        {
          id: "2",
          imageUrl: "http://www.gunshopschweiz.ch/Product/Show/6468",
          productName: "Standard Manufacturing S333",
          price: "1562.-",
          releasedDate: "October 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 2,
        },
        {
          id: "3",
          imageUrl: "http://www.gunshopschweiz.ch/Product/Show/6580",
          productName: "SIG SAUER Cross",
          price: "2203.-",
          releasedDate: "May 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 5,
        },
        {
          id: "4",
          imageUrl: "http://www.gunshopschweiz.ch/Product/Show/6357",
          productName: "Maschinengewehr Degtjarjow",
          price: "1153.-",
          releasedDate: "May 1, 1233",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 4,
        },
        {
          id: "5",
          imageUrl: "http://www.gunshopschweiz.ch/Product/Show/5467",
          productName: "IWI Tavor",
          price: "2093.-",
          releasedDate: "October 31, 1980",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 2,
        },
        {
          id: "6",
          imageUrl: "http://www.gunshopschweiz.ch/Product/Show/5366",
          productName: "SIG SAUER P320 Spectre",
          price: "6783.-",
          releasedDate: "May 3, 2021",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 5,
        },
      ],
    };
  },
};
</script>

<template>
  <div v-for="product in products" :key="product.id">
    <Product :data="product" />
  </div>
</template>
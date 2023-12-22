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
          imageUrl: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/M%C3%A5lskjutningspistol%2C_1910_cirka_-_Livrustkammaren_-_100366.tif/lossy-page1-1280px-M%C3%A5lskjutningspistol%2C_1910_cirka_-_Livrustkammaren_-_100366.tif.jpg",
          productName: "Taurus Raging Bull (2-454089M)",
          price: "1231.-",
          releasedDate: "May 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 4,
        },
        {
          id: "2",
          imageUrl: "https://preview.redd.it/jt6pdpwlmw7c1.jpeg?width=640&crop=smart&auto=webp&s=809176921fb7909d998679b058e62cd2843e5817",
          productName: "Standard Manufacturing S333",
          price: "1562.-",
          releasedDate: "October 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 2,
        },
        {
          id: "3",
          imageUrl: "https://preview.redd.it/heta2hahz4ea1.jpg?width=640&crop=smart&auto=webp&s=ff429a857b74c5bec8ecf0d1a591a0e9bd73e48c",
          productName: "SIG SAUER Cross",
          price: "2203.-",
          releasedDate: "May 31, 2023",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 5,
        },
        {
          id: "4",
          imageUrl: "https://preview.redd.it/vr7mublb4a9a1.jpg?width=640&crop=smart&auto=webp&s=2f575e567ab749d2db17cfbfef6122d0c19fa7af",
          productName: "Maschinengewehr Degtjarjow",
          price: "1153.-",
          releasedDate: "May 1, 1233",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 4,
        },
        {
          id: "5",
          imageUrl: "https://preview.redd.it/jp37o03voxoa1.jpg?width=640&crop=smart&auto=webp&s=9f0ba9d099cfccfea32b66cd84483fa808fa4668",
          productName: "IWI Tavor",
          price: "2093.-",
          releasedDate: "October 31, 1980",
          description: "Lorem ipsum dolor sit amet, consctetur...",
          rating: 2,
        },
        {
          id: "6",
          imageUrl: "https://external-preview.redd.it/bhON5T1CRUPIIU5_1jmTK7nbT_c7SN5Z-IoAxiw7_gI.jpg?width=640&crop=smart&auto=webp&s=d65576c4174a0d852ae3dc4293cf2f228101b02b",
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
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
          imageUrl: "https://i.redd.it/mb0soceyck141.jpg",
          productName: "Wolkenroller",
          releasedDate: "April 31, 2030",
          description: "Luftig und fliegt regelrecht über die Kurven",
          rating: 4,
        },
        {
          id: "2",
          imageUrl: "https://i.imgur.com/EVCwQNR.jpeg",
          productName: "D-Klasse 1/2",
          releasedDate: "June 31, 2003",
          description: "Klein aber Fein",
          rating: 2,
        },
        {
          id: "3",
          imageUrl: "https://i.quotev.com/tinohuzkngpa.jpg",
          productName: "Gesichtsklasse",
          releasedDate: "February 31, 2093",
          description: "Der Kopf eines Mannes und das Auto ein langes",
          rating: 5,
        },
        {
          id: "4",
          imageUrl: "https://a-static.mlcdn.com.br/450x450/hot-wheels-octane-rocket-league-fyf57/maonaroda4x4/5812150007/84c5eb35f0ae18dc76b9d5fb22c74506.jpg",
          productName: "Raketenwagen",
          releasedDate: "November 31, 2023",
          description: "Das Spielzeug eines wahren Mannes",
          rating: 2,
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

<style>  
.productName {
  font-size:4;
}

.description {
  font-size:2,5;
}

.rating {
  font-size:3;
}
</style>





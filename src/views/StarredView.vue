<script setup lang="ts">
import FrameworkPop from "@/components/FrameworkPop.vue";
const fremeList = [
  {
    name: "VueJS",
    img: "https://masteringjs.io/assets/images/vue/vue.png",
    rating: 10,
  },
  {
    name: "AngularJS",
    img: "https://angular.io/assets/images/logos/angularjs/AngularJS-Shield.svg",
    rating: 20,
  },
  {
    name: "ReactJS",
    img: "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/2300px-React-icon.svg.png",
    rating: 14,
  },
];
</script>

<template>
  <v-container>
    <v-row>
      <v-col v-for="(item, index) of fremeList" :key="index">
        <FrameworkPop
          :name="item.name"
          :img="item.img"
          :rating="item.rating"
        ></FrameworkPop
      ></v-col>
    </v-row>
  </v-container>
</template>

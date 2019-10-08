<template>
  <ul>
    <li v-for="dog in dogs" :key="dog.id">
      <DogListing @click.native="upvoteDog(dog.id)" :dog="dog" />
    </li>
  </ul>
</template>

<script>
import DogListing from "@/components/DogListing";
export default {
  components: {
    DogListing
  },
  props: {
    dogs: Array
  },
  methods: {
      upvoteDog(id){
          
      }
  }
};
</script>

<style lang="scss">
.dogList {
  ul {
    list-style: none;
  }
}
</style>
<template>
  <div class="dog-listing">
    <img :src="dog.imageUrl" alt="dog" />
    <h3>{{dog.name}}</h3>
  </div>
</template>
<script>
export default {
  props: {
    dog: Object
  }
};
</script>

<style lang="scss">
.dog-listing {
  margin-bottom: 2rem;
  img {
    width: 100px;
  }
  h3 {
    padding: 0;
    margin: 0;
  }
}
</style>
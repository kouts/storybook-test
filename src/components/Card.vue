<template>
  <div class="card" style="width: 18rem;">
    <div v-if="headerTitle" class="card-header">
      {{ headerTitle }}
    </div>    
    <img src="lion.jpg" class="card-img-top" alt="Lion" />
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">
        Some quick example text to build on the card title and make up the bulk
        of the card's content.
      </p>
      <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    headerTitle: {
      type: String,
      default: ''
    },
    title: {
      type: String,
      default: 'Card title'
    },
    content: {
      type: String,
      default: 'Some quick example text to build on the card title and make up the bulk of the card\'s content.'
    }
  }
};
</script>

<style>
</style>

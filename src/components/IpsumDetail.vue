<template>
  <section v-if="ipsum" class="detail-container">
    <div class="detail">
      <h3>{{ipsum.title}}</h3>
      <p v-html="ipsum.body"></p>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    ipsum: Object
  }
};
</script>

<style>
.detail-container {
  padding: 15px;
}
.detail {
  border: 2px solid black;
  object-fit: contain;
  overflow: scroll;
  height: 200px;
}
</style>

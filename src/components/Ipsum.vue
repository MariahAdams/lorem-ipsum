<template>
  <section>
    Ipsum Component
    <div>
      <IpsumDetail :ipsum="ipsum"/>
    </div>
    <div>
      <h2>Please select an Ipsum:</h2>
    </div>
  </section>
</template>

<script>
import IpsumDetail from './IpsumDetail';

export default {
  props: {
    ipsum: Object
  },
  components: {
    IpsumDetail
  }
};
</script>

<style>

</style>

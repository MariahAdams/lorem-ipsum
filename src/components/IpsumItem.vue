<template>
  <li>
    <h3>{{ipsum.title}}</h3>
    <p>{{ipsum.category}}</p>
  </li>
</template>

<script>
export default {
  props: {
    ipsum: Object
  }
};
</script>

<style>
li {
  border: 2px solid black;
}
</style>

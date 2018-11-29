<template>
  <ul>
    <IpsumItem />
  </ul>
</template>

<script>
import IpsumItem from './IpsumItem';

export default {
  props: {
    ipsums: Array
  },
  components: {
    IpsumItem
  }
};
</script>

<style>
ul {
  list-style: none;
}
</style>

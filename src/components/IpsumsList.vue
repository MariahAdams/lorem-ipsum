<template>
  <ul>
    <IpsumItem 
      v-for="ipsum in ipsums"
      :key="ipsum.title"
      :ipsum="ipsum"
    />
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
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  grid-gap: 50px;
}
</style>
